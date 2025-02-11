# zeno_indexing_*

A multi-language implementation of 
David Greenspan's [fractional indexing implementation](https://observablehq.com/@dgreensp/implementing-fractional-indexing@547) 
with the following goals:

 * a unique (and ironic) name (see Zeno's [dichotomy paradox](https://en.wikipedia.org/wiki/Zeno%27s_paradoxes#Dichotomy_paradox)),
 meant to dispel the idea that it's byte-for-byte compatible with other implementations of Greenspan's algorithm

 * a common test suite, so if there's a bug, we can test it and patch across
 the implementations

 * all implementations are versioned together — striving for compat between
 major and minor versions


# Supported Languages

 * Elixir (see [zeno_indexing_ex](./elixir))
 * Javascript (see [zeno_indexing_js](./typescript)) written in Typescript

## Background

`zeno_indexing_*` was initially written in the context of [StepTree](https://www.steptree.co)
where browser code could generate a fractional index, and at times, so could its
backend server, written in Elixir.


## Contributing

If you'd like to add a language, feel free to suggest a pull request in a 
new folder. My hope is for the test suite to help maintain compatiblity.

The test cases are generated in an Elixir script (see [./elixir/scripts/README.md](./elixir/scripts/README.md)) and stored in [`./test_cases.json`](./test_cases.json)
