# zeno_indexing_*

A multi-language implementation of 
David Greenspan's [fractional indexing implementation](https://observablehq.com/@dgreensp/implementing-fractional-indexing@547) 
with the following goals:

 * share a test suite across implementations, so if a bug is uncovered, we can test it and patch across
 the implementations

 * all implementations are versioned together — striving for compat between
 major and minor versions

# Language implementations


 * Elixir (see [zeno_indexing_ex](https://github.com/gdso/zeno_indexing_ex))
 * TODO Javascript 


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
