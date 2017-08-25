<p align="center">
  <img width="556" height="112" src="https://github.com/ShikharJ/GSoC-2017-Work-Report/blob/master/src/gsoc.png">
</p>

[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/sympy/symengine?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

My proposal for **Improving SymEngine's Python Wrappers and SymPy-SymEngine Integration** was selected as an official project under **Google Summer of Code 2017**. I worked with the organisation [SymPy](https://github.com/SymPy/), under the mentorship of **Isuru Fernando** ([@isuruf](https://github.com/isuruf)) and **Sumith Kulal** ([@sumith1896](https://github.com/sumith1896)).

## Goal

`SymPy` is a `Python` based library for Symbolic Mathematics. It aims to become a full-featured Computer Algebra System (CAS) while keeping the code as simple as possible in order to be comprehensible and easily extensible.
The `SymPy` organization also supports `SymEngine`, a standalone fast `C++` symbolic manipulation library with wrappers in many languages, including `C`, `Python`, `Ruby`, `Julia` and `Haskell`.

Speed is of the utmost importance for any CAS.

`SymEngine`, was initially developed with the aim of serving as an optional core for the `SymPy` CAS in the future. Over the years, it has matured enough to be used as a symbolic backend. Using `SymEngine` can significantly increase speeds of various symbolic operations, and hence make `SymPy` an ideal choice for projects requiring fast manipulations, by giving them the option to switch over to `SymEngine`’s routines.

On the other hand, this will also lead to the development of a number of features currently lacking in `SymEngine` and its `Python` wrapper, which would be ported over from `SymPy` in order to provide smooth wrappers for optional use.

## Results

### Links To Commits

[SymEngine](https://github.com/symengine/symengine/commits?author=shikharj)


[SymEngine.py](https://github.com/symengine/symengine.py/commits?author=shikharj)

<p align="left">
  <img width="459" height="198" src="https://github.com/ShikharJ/GSoC-2017-Work-Report/blob/master/src/SymEnginepy.jpg">
</p>

[SymPy](https://github.com/sympy/sympy/commits?author=shikharj)


## Scope and Future Work

Work on this project is far from over. `SymPy` codebase is huge, and given the number of active contributors and beneficiaries, it's only going to increase and incorporate more and more functionalities in the future. During this summer, only the functionalities that were common to `SymEngine` and `SymPy` were ported over through `SymEngine.py`. However, still, a gargantuan amount of assertion failures, exceptions and inconsistencies had to be resolved to finally get the code running, which took up a lot of time during this project. We still currently don't have the assumptions and calculus module available in `SymEngine`, both being full-length `GSoC` projects on their own. Hence, this work is expected to continue for the time to come.

## Conclusion

I have no words to describe how grateful I am to my mentors - [Isuru Fernando](https://github.com/isuruf) and [Sumith Kulal](https://github.com/Sumith1896) - for all their support and for being extremely responsive and helpful with every one of my problems. Without their vote of confidence, this project would've been a lot harder and a lot less fun to do.

I would be lucky to get to work with them further as I continue work on this project till the time `SymEngine` becomes the default core of the `SymPy` library.

I am also thankful to `SymPy` and `Google` for the opprtunity to work on this project, which helped me learn a lot in such a short period of time.
