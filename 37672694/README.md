[View on StackOverflow](https://stackoverflow.com/a/51924868/7602110)

This is **weird** but this is how I do it!

I have a repository on [Github][1] but I wanted to use the [Gitlab][2] CI, so I mirrored the repository from **Github** to **Gitlab**, then I configured the CI etc... I was looking around online, and I found that with Gitlab Enterprise you have [the feature][3] of pushing changes to an external repository from **GitLab**, but since I don't pay for Gitlab Enterprise, I did the following:

Since we are using [GIT][4], and we <s>are good programmers</s> try to be good programmers make it work, so:

**I JUST EDITED THE GIT URL**

How was it?

- Clone your repository
- Go to your project ...
- Navigate to `.git` **>** `config` and you should have something like this!

   [![.git/config file][5]][5]

Change the **URL** from **Github** to **Gitlab** (I had the same username and project name, in both services so, I only changed the URL).

Then with the **Gitlab** URL:

`git pull origin`

Since the remote URL have changed, you should get the changes from **Gitlab**.

- Change again your remote URL back again to **Github**
- Then push your changes

`git pull origin`

You should be done! Hope the trick works for you, it did work for me, so.. 🧐

  [1]: https://github.com/abranhe/ci-success/
  [2]: https://gitlab.com/abranhe/ci-success/
  [3]: https://about.gitlab.com/2016/05/10/feature-highlight-push-to-remote-repository/
  [4]: https://git-scm.com/
  [5]: https://i.stack.imgur.com/1n8T3.png
