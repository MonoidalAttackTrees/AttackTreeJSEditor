# AttackTreeJSEditor
An editor for building attack trees written in Javascript.

Installing GHCJS on GHC 8.0.1
-----------------------------

- Clone the GHCJS repo:
  ``git@github.com:ghcjs/ghcjs.git``

- Checkout the ``ghc-8.0`` branch.

- These programs must be installed: autoconf and automake
  It is easiest to use [homebrew](https://brew.sh/) to install these programs.

- Inside the ghcjs repo run the following to install it:
  ``cabal install .``

- Now bootstrap GHCJS using the following command inside the ghcjs repo:
  ``ghcjs-boot --dev --ghcjs-boot-dev-branch ghc-8.0 --shims-dev-branch ghc-8.0``
  Warning: the previous command builds *all* of ghcjs.  Make sure you have plenty of time before running.