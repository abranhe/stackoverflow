[View on StackOverflow](https://stackoverflow.com/a/52125181/7602110)

The easiest way to get the current user name is definitely **[`username`][1]**.

`pip install username`

then:

```py
import username
    
print(username())
# your_username
```

And there is also [`username-cli`][2], a **CLI** tool to get your username, just:

`pip install username-cli`

then:

```console
$ username
# -> your username
```

> Works on Linux, macOS, and Windows 

  [1]: https://pypi.org/project/username
  [2]: https://pypi.org/project/username-cli
