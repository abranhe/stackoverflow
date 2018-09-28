[View on StackOverflow ..](https://stackoverflow.com/a/47901334/7602110)

Remove your user settings:

Name: `$~ git config --global --unset user.name`

Email: `$~ git config --global --unset user.email`

or all your global settings:

`$~ git config --global --unset-all`

Then [set your username][1]  in git.

To check who you are:

`$~ git config --list`


[1]: https://help.github.com/articles/setting-your-username-in-git/
