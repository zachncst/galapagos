# galapagos

An implementation of the GraphQL specification in Clojure.

[![Build Status](https://travis-ci.org/jstaffans/galapagos.svg?branch=master)](https://travis-ci.org/jstaffans/galapagos)

## Overview

The goal of this library is to expose the data of your Clojure application in a way that enables
GraphQL clients to interact with it. Special care is taken to make data access as efficient as possible - 
streamlined, concurrent data fetching is provided by the [muse](https://github.com/kachayev/muse) library.

See [links](https://github.com/jstaffans/galapagos/blob/master/links.md) for more information on GraphQL and the ideas behind it.

## Development

To help in understanding the internals of Galapagos, there's an [annotated overview](http://jstaffans.github.io/galapagos/) of the
source code in the spirit of literate programming.

## Status

Galapagos is still very much pre-alpha software and nearly everything is subject to change.

### Schema definition

The schema definition DSL is still a work-in-progress and a bit clunky in places.

### Queries

Directives and query variables are missing. Validation is lacking.
Support for muse's query batching (a solution to the [1+N query problem] [1]) is not yet implemented.

### Mutation

Mutation operations are not currently supported.

## License

Distributed under the MIT License - see LICENSE for the full license.

[1]: https://github.com/kachayev/muse/blob/master/docs/sql.md
