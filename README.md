# Issue

https://github.com/lukeed/ley/issues/6

Run `yarn && yarn migrate`.

`ley` should show connection errors in the terminal but they are swallowed instead.

Issue is fixed when using `postgres@^1` or when commenting out the `catch` in https://github.com/porsager/postgres/blob/master/lib/index.js#L250
