# example trapperkeeper app

Heavily-commented scaffold trapperkeeper app generated via `lein new trapperkeeper`

## Usage

First, run:

    $ lein tk

Then, open a browser and visit: `http://localhost:8080/hello/example`

### Running from the REPL

Alternately, run:

    $ lein repl
    nREPL server started on port 52137 on host 127.0.0.1
    user => (go)

This will allow you to launch the app from the Clojure REPL. You can then make
changes and run `(reset)` to reload the app or `(stop)` to shutdown the app.

In addition, the functions `(context)` and `(print-context)` are available to
access or print out the current trapperkeeper application context. Both of these take an
optional array of keys as a parameter, which is used to retrieve a nested
subset of the context map.

Try `(keys (context))` to see the top-level keys.
Try `(context [:service-contexts :ConfigService])` to
fetch the `:service-contexts` entry in the context, and
fetch the `:ConfigServices` entry from that.

## License

Copyright © 2019 FIXME

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.
