[View on StackOverflow ..](https://stackoverflow.com/a/52322780/7602110)

Definitely, the easiest way to do it is using [`username`][1]

### Install:

    $ npm install username

### Then:

    const username = require('username');

    (async () => {
	    console.log(await username());
    	//=> 'current_username'
    })();

  [1]: https://github.com/sindresorhus/username
