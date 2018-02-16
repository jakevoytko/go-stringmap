What?
-----

A wrapper around github.com/go-redis/redis' implementation of hashes.

But just the parts of the interface that I use. I wouldn't want it to be *too* useful.

Also provides a working in-memory version to use in tests.

Why?
----

I wanted to use this wrapper in 2 projects. Releasing it as its own repository
is kind of an experiment, given the fact that its a trivial
implementation. Don't want this to turn into NPM hell.