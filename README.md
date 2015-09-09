# docker-clojure-ring

A Dockerfile, building off the official
[Clojure image](https://hub.docker.com/r/library/clojure/), but adding
the [Lein Ring](https://github.com/weavejester/lein-ring) plugin.

For example, to build an uberjar for a Ring app, run:

    $ docker run -it --rm -v "$PWD":/usr/src/app -w /usr/src/app clojure lein ring uberjar
