# zeno_indexing_*

A multi-language implementation of 
David Greenspan's [fractional indexing implementation](https://observablehq.com/@dgreensp/implementing-fractional-indexing@547) 
with the following goals:

 * share a test suite across implementations, so if a bug is uncovered, we can test it and patch across
 the implementations

 * all implementations are versioned together — striving for compat between
 major and minor versions

# Language implementations


 * Elixir (see [zeno_indexing_ex](./elixir))
 * Javascript (see [zeno_indexing_js](./typescript)) written in Typescript


## Contributing

If you'd like to add a language, feel free to suggest a pull request in a 
new folder. My hope is for the test suite to help maintain compatiblity.

The test cases are generated in an Elixir script (see [./elixir/scripts/README.md](./elixir/scripts/README.md)) and stored in [`./test_cases.json`](./test_cases.json)

## FAQ

### Q: Why yet another fractional indexing library?

`zeno_indexing_*` was initially written in the context of [StepTree](https://www.steptree.co)
where client/browser code could generate a fractional index. Over time, for conflict resolution as well for testing, 
it became clear that the backend server, written in Elixir, would have to generate fractional indices as well.


At the time of its writing, I didn't know 
of any Elixir implementations, and I was afraid it might drift by accident or on purpose 
from the Javascript implementations out there, so I decided to take matters into my own hands.

### Q: What's with the name?

Well I wanted to pick a unique name, and I do think Zeno's [dichotomy paradox](https://en.wikipedia.org/wiki/Zeno%27s_paradoxes#Dichotomy_paradox)
is analogous to how in theory fractional indexing works, assuming we had infinitely precise floating point numbers, of course!
