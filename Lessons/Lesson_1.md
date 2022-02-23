-- *Slide* --
### Part 0: Goals for today
* Part 1: Python and HPC Environments
* Part 2: Job Submission with Python
* Part 3: Parallel Python
* Part 4: Optimising Python
-- *Slide End* --

-- *Slide* --
### Part 0: Slide Respository
* A copy of the slides and same code is available at: https://github.com/levlafayette/SpartanPython
* Make use of our resources: `dashboard.hpc.unimelb.edu.au`,  `hpc-support@unimelb.edu.au`, `man spartan`
* Especially `/usr/local/common/Python`
-- *Slide End* --

-- *Slide* --
### Part 1: The Python Story
* Python is a very popular high-level programming language. Top of the Tiobe index (Feb 2022)
* First released in 1991 byGuido van Rossum at Centrum Wiskunde & Informatica (CWI) in the Netherlands
* v2.0 in 2000 with better memory management (garbage collector) and Unicode support. v3.0 first ever intentionally backwards incompatible (print as a function, APIs such views and iterators used in instead Of lists), text and binary rather than unicode and 8-bit.
* Named after "Monty Python's Flying Circus", which Guido was reading at the time. 
-- *Slide End* --

-- *Slide* --
### Part 1: Python Design
* Designed for code readability, object-orientated approach, dynamically-typed,  dynamic name resolution.
* Design principles encapsulated in "Zen of Python" by Tim Peters; major elements include: Beautiful is better than ugly, Explicit is better than implicit, Simple is better than complex, Complex is better than complicated, Readability counts,  Flat is better than nested, Errors should never pass silently (Unless explicitly silenced), There should be one – and preferably only one – obvious way to do it (a dig at Perl), If the implementation is hard to explain, it's a bad idea.
-- *Slide End* --

-- *Slide* --
<img src="https://raw.githubusercontent.com/levlafayette/SpartanParallel/master/Images/python_environment.png" height="200%" width="200%" />
-- *Slide End* --

-- *Slide* --
### Part 1: Versions and Extensions
* Python has many release versions, more than 200,000 extensions known as "packages", and a number of installation methods and environments. This can be is complex and confusing.
* The basic and recommended approproach on Spartan is the modules system for the core language and some packages. e.g., `module -r avail '^python'`, `module avail scipy-bundle`, `module avail numpy`
* Because there are so many packages we often suggest that users install them in their own environment.
-- *Slide End* --

-- *Slide* --
### Part 1: Environments
* Python environments are used to create a self-contained directory tree that has application coherence (so the requirements of application A don't conflict with those for application B).
* This is possible with modules, most popular user tools are VirtualEnv and Conda. Whilst popular there are many problems with using these on an HPC, including default install location and environment changes. 
-- *Slide End* --

-- *Slide* --
<img src="https://raw.githubusercontent.com/levlafayette/SpartanParallel/master/Images/squarematrixmultiply.png" height="200%" width="200%" />
-- *Slide End* --

-- *Slide* --
### Part 1: Python Is Slow
* For a sample computationally-intensive problems (a square matrix multiplication), Java is 8.8x faster than Python, CLang is 18x faster. Difference between an interpreted language versus a byte-code with JiT compilation, versus compilation to machine-code.
* Similar results when comparing overall energy efficiency; runtime, memory usage, energy consumption (CPU, DRAM). Compared against 27 programming languages, Python came last. Compiled languages (C, C++, Fortran, Rust, Pascal) were best. Interpreted languages like Python, Perl, Lua, Ruby were the worst. 
-- *Slide End* --




-- *Slide* --
<img src="https://raw.githubusercontent.com/levlafayette/SpartanParallel/master/Images/hypnotoad.png" height="200%" width="200%" />
-- *Slide End* --


