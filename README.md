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

How?
----

```
go get -u github.com/jakevoytko/stringmap
```

For examples of usages in test and programs, see github.com/jakevoytko/crbot.

Potential changes
-------------------

I've considered caching the map in-memory and doing asynchronous writes. I would
provide that as an opt-in option, so I don't expect the behavior to change at
all.