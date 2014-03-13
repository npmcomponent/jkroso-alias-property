*This repository is a mirror of the [component](http://component.io) module [jkroso/alias-property](http://github.com/jkroso/alias-property). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/jkroso-alias-property`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# alias-property

  create robust aliases for an object's properties

## Installation

_With [packin](//github.com/jkroso/packin) or [component](//github.com/component/component)_

    $ packin add jkroso/alias-property

then in your app:

```js
var alias = require('alias-property')
```

## API

### alias(obj, to, from)

  create an alias from `from` to `to`

```js
var obj = {a:1};
alias(obj, 'a', 'b');
obj.a; // => 1
obj.b; // => 1
obj.b = 2;
obj.a; // => 2
obj.b; // => 2
obj.a = 3;
obj.a; // => 3
obj.b; // => 3
```

## Running the tests

Just run `make` and navigate your browser to the test directory.
