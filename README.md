Underscore.js assertion helper
==============================

- This is not for tests files project,
- This is not instead of [jasmine][2] or any test framework,
* This is for test in production code!

Usage
=====

```javascript
_.assert(typeof fn === 'function', '*fn* should be function');
// throws AssertionError

_.assert(list.length, '*list* should contains any value');
// for non-empty list nothing do it, but for empty list throw AssertionError
```

Example
=======
```javascript
function isUrl(url) {
  _.assert(typeof url === 'string', 'URL should be a *string* value');
  // ... valid URL
}
```

<pre>


Dependencies [underscore][1].
                         _
                        | |
  __ _ ___ ___  ___ _ __| |_
 / _` / __/ __|/ _ \ '__| __|
| (_| \__ \__ \  __/ |  | |_
 \__,_|___/___/\___|_|   \__|
</pre>

Changelog
=========

- Added `assert` method to main `_` underscore namespace.
Method throws AssertionError if first param is not boolean `true`.

License
=======

[The MIT License][3]

[1]: http://underscorejs.org/
[2]: http://pivotal.github.io/jasmine/
[3]: https://github.com/piecioshka/underscore-assert/blob/master/LICENSE