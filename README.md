# ~/.clojure/

My user level configuration for Clojure CLI tools heavily inspired by [Sean Corfield's `deps.edn`](https://github.com/seancorfield/dot-clojure) and [Practicalli deps.edn](https://github.com/practicalli/clojure-deps-edn).

# Aliases

## `:env/dev`

Include `dev` directory on the class path. Supports the use of `dev/user.clj` to [configure REPL startup](http://practicalli.github.io/clojure/clojure-tools/configure-repl-startup.html).

## `:project/new`

Create a new project with [`clj-new`](https://github.com/seancorfield/clj-new) based on a template.

To create an app:

    $ clojure -M:project/new app eploko/my-app
    
To create a lib:

    $ clojure -M:project/new lib eploko/my-lib
    
More examples:

    $ clojure -M:project/new luminus eploko/full-stack-app +http-kit +h2 +reagent +auth
    
## `:repl`

Reveal REPL with nrepl server and Emacs CIDER specific middleware. Use with `M-x cider-connect-clj` in Emacs.
