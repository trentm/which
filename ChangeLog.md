## v1.1.0 ##

  * Change version attributes and semantics. Before: had a `_version_` tuple. After: `__version__` is a string, `__version_info__` is a tuple.

## v1.0.3 ##

  * Move hosting of `which.py` to trentm.com. Tweaks to associated bits (README.txt, etc.)

## v1.0.2 ##

  * Rename mainline handler function from `_main()` to `main()`. I can conceive of it being called from externally.

## v1.0.1 ##

  * Add an optimization for Windows to allow the optional specification of a list of exts to consider when searching the path.

## v1.0.0 ##

  * Simpler interface: What was which() is now called whichgen() -- it is a generator of matches. The simpler which() and whichall() non-generator interfaces were added.

## v0.8.1 ##

  * API change: 0.8.0's API change making "verbose" output the default was a mistake -- it breaks backward compatibility for existing uses of which in scripts. This makes verbose, once again, optional but NOT the default.

## v0.8.0 ##

  * bug fix: "App Paths" lookup had been crippled in 0.7.0. Restore that.
  * feature/module API change: Now print out (and return for the module interface) from where a match was found, e.g. "(from PATH element 3)".  The module interfaces now returns (match, from-where) tuples.
  * bug fix: --path argument was broken (-p shortform was fine)

## v0.7.0 ##

  * bug fix: Handle "App Paths" registered executable that does not exist.
  * feature: Allow an alternate PATH to be specified via 'path' optional argument to which.which() and via -p|--path command line option.

## v0.6.1 ##

  * first public release