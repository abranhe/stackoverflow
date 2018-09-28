[View on StackOverflow](https://stackoverflow.com/a/51165669/7602110)

I had the same issue and I tried some of the above answers, maybe they are ok, but none of those answers fixed on what I was trying to do it, using macOS. I was trying to iterate over dates in the past.

**I am using macOS**, and the following is what worked for me:

    #!/bin/bash

    # Get the machine date
    newDate=$(date '+%m-%d-%y')

    # Set a counter variable
    counter=1

    # Increase the counter to get back in time
    while [ "$newDate" != 06-01-18 ]; do
      echo $newDate
      newDate=$(date -v -${counter}d '+%m-%d-%y')
	  counter=$((counter + 1))
    done

Hope it helps.Â
