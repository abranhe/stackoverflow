[View on StackOverflow](https://stackoverflow.com/a/52338821/7602110)

You can install [`permutated`](https://github.com/abranhe/permutated)

### Installing

`$ npm install permutated`

### Usage

    const permutated = require('permutated');

    (async () => {
	    console.log(await permutated('abc'));
    	//=> [ 'abc', 'acb', 'bac', 'bca', 'cab', 'cba' ]
    })();
