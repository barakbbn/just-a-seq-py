# just-a-seq-py [![GitHub last commit](https://img.shields.io/github/last-commit/barakbbn/just-a-seq-py)](https://github.com/barakbbn/just-a-seq-py) [![GitHub license](https://img.shields.io/github/license/barakbbn/just-a-seq-py)](https://github.com/barakbbn/just-a-seq-py/LICENSE)

This is just a **sequence** that provides LINQ functionalities (and more)  
But with an API that resembles Python list and itertools ( `map()` instead of `Select()`, `filter()` instead of `Where()`).  
It wraps a list or other Iterable object or a Generator.  (`asSeq([1,2,3])` , `asSeq(range(1, 10))`)

---

### Features

* Type Hinting
* Fluent API - chain functions calls to simplify the code:  `seq.filter().map().sorted().to_list()`
* Lazy/Deferred functionalities, like Python itertoools and .NET LINQ.
* Sequence can be iterated more than once

  Instead of immediately producing a new `list` from methods such as `map`, `filter`, it iterates the items only once
  when being consumed (i.e. for..loop,  `.to_list()`, `.foreach()`, `.count()` ).
* Immutable - actions on the sequence won't change it, but return a new sequence with the changes
* API that more resemble to Python list and itertools
  (Since most existing libraries already mimics .Net IEnumerable).
* Additional useful functionalities that can make you more productive.
