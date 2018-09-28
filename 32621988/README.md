[View on StackOverflow](https://stackoverflow.com/a/52306523/7602110)

I face the same issue and this worked for me!

Install [jQuery](https://www.npmjs.com/package/jquery) using **npm**

    npm i jquery


Then include jQuery in one of the following ways.

> Using Script tag

    <script>window.$ = window.jQuery = require('jquery');</script>

> Using Babel

    import $ from "jquery";

> Using Webpack

    var $ = require('jquery')
