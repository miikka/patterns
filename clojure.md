# Clojure and ClojureScript


## Default library choices

* Promises for JVM: [manifold.deferred](http://aleph.io/manifold/deferreds.html)
* Promises for the browser: [promesa](https://funcool.github.io/promesa/latest/)
* Data manipulation utility belt: [potpuri](https://github.com/metosin/potpuri) and/or [specter](https://github.com/nathanmarz/specter)

Boot plugins:

* Running Clojure tests: [boot-alt-test](https://github.com/metosin/boot-alt-test)


## Release process for open-source libraries

* Check that the changelog is up-to-date.
* Create a git tag. Remember to push it!
* Sign the JAR (and make sure you've published your public key).
* After making a release, increase the version number to a `-SNAPSHOT` version.
* If possible, use `lein release` which automatically takes care of the tag and the version number.
