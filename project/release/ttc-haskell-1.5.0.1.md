# `ttc-haskell` `1.5.0.1` Release Notes

Date
: 2026-01-10

## Overview

TTC, an initialism of _Textual Type Classes_, is a library that provides the
following functionality:

* The `Textual` type class is used to convert between common textual data
  types.  It can be used to write functions that accept or return values of
  any of these textual data types.
* The `Render` type class is used to render a value as text.  Avoid bugs by
  only using `Show` for debugging/development purposes.
* The `Parse` type class is used to parse a value from text.  Unlike `Read`,
  it has support for error messages.
* Validate constants at compile-time using `Parse` instances.

See the [README][] for details.

[README]: <https://github.com/ExtremaIS/ttc-haskell#readme>

## This Release

This is a maintenance release that adds compatibility with GHC 9.14.1.  There
are no changes to the API or CLI.

### Compatibility

GHC versions 8.8.4 through 9.14.1 are supported.  Note that GHC 9.12.3 is not
tested, however, because it has critical issues and is not available using
GHCup.

Cabal version 3.0 through 3.16.1.0 are supported.

To use this release with a Stackage snapshot that does not include it, add
the following to your `stack.yaml` configuration:

```yaml
extra-deps:
  - ttc-1.5.0.1
```

### Issues

There are no known issues at this time.
