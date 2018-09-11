[See it on Stackoverflow ...](https://stackoverflow.com/a/52266386/7602110)

Pretty simple using `map`! 

> See the [Repl.it](https://repl.it/@abranhe/mapExample)

```cpp
#include <iostream>
#include <map>

int main()
{
    int foo[]{1,1,1,1,4,6,4,7,4};
    std::map<int, int> bar;

    for (auto const &f : foo)
        bar[f]++;

    for (auto const &b : bar)
        std::cout << "The number " << b.first 
                  << "is repeated " << b.second 
                  << "times\n";
}
```

Expected output:

```
The number 1 is repeated 4 times
The number 4 is repeated 3 times
The number 6 is repeated 1 times
The number 7 is repeated 1 times
```
