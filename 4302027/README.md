[View on StackOverflow](https://stackoverflow.com/a/52284689/7602110)

On **window**

    import os
    os.system("start \"\" https://example.com")

On **macOS**

    import os
    os.system("open \"\" https://example.com")

On **Linux**

    import os
    os.system("xdg-open \"\" https://example.com")

**Cross-Platform**

    import webbrowser

    webbrowser.open('https://example.com')
