# expose-mongo-result

Meteor’s mongo-livedata package as of 0.6.5.1, patched to include the
Mongo database result in collection method calls on the server.

The Mongo database result is needed for some of the more advanced
atomic update techniques, such as
[Update if Current](http://docs.mongodb.org/manual/tutorial/isolate-sequence-of-operations/#update-if-current).

This patch is also available as a pull request:
https://github.com/meteor/meteor/pull/1421

To use, create the packages directory if needed:

    $ mkdir packages

and then clone this repository into `packages/mongo-livedata`:

    $ git clone https://github.com/awwx/meteor-expose-mongo-result.git packages/mongo-livedata

This will override the standard Meteor mongo-livedata package with
this one.
