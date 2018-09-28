[View on StackOverflow](https://stackoverflow.com/a/52547414/7602110)

I would use the `reverse()` function from the `<algorithm>` library.

Run it online: [repl.it/@abranhe/Reverse-Array](https://repl.it/@abranhe/Reverse-Array)


    #include <iostream>
    #include <algorithm>
    using namespace std;

    int main()
    {
      int arr [10] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

      reverse(begin(arr), end(arr));

      for(auto item:arr)
      {
        cout << item << " ";
      }
    }

Output:

    10 9 8 7 6 5 4 3 2 1

Hope you like this approach.
