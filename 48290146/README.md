[View on StackOverflow](https://stackoverflow.com/a/48290292/7602110)

You can read a file anywhere on your computer, here is an example using Java **BufferedReader**

    import java.io.BufferedReader;
    import java.io.FileReader;
    import java.io.IOException;

    public class ReadFileExample1 {

	  private static final String FILENAME = "E:\\test\\filename.txt";

	    public static void main(String[] args) {

		BufferedReader br = null;
		FileReader fr = null;

		try {
			//br = new BufferedReader(new FileReader(FILENAME));
			fr = new FileReader(FILENAME);
			br = new BufferedReader(fr);

			String sCurrentLine;

			while ((sCurrentLine = br.readLine()) != null) {
				System.out.println(sCurrentLine);
			}

		} catch (IOException e) {
			e.printStackTrace();
		} finally {
          try {
			  if (br != null) br.close();
			  if (fr != null) fr.close();
		  } catch (IOException ex) {
			  ex.printStackTrace();
		  }
		}
	  }
    }

 View [tutorial](https://www.mkyong.com/java/how-to-read-file-from-java-bufferedreader-example/) useful to read from files.
