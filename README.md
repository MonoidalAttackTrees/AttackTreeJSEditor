# AttackTreeJSEditor
An editor for building attack trees written in Javascript.

Installing GHCJS on Mac OS X with GHC 8.0.1 
-------------------------------------------

- Clone the GHCJS repo: ``git clone git@github.com:ghcjs/ghcjs.git``

- Checkout the ``ghc-8.0`` branch: ``git checkout ghc-8.0``

- These programs must be installed: autoconf and automake

  It is easiest to use [homebrew](https://brew.sh/) to install these programs.

- Install [node.js](https://nodejs.org/en/download/).

  Note: Use the offical download from the node js website instead of brew, because the version in brew is old.

- Inside the ghcjs repo run the following to install it: ``cabal install .``

- Now bootstrap GHCJS using the following command inside the ghcjs repo:

  ``ghcjs-boot --dev --ghcjs-boot-dev-branch ghc-8.0 --shims-dev-branch ghc-8.0``

  Warning: the previous command builds *all* of the ghcjs libraries.  Make sure you have plenty of time before running it.