# DBSystem-Concepts

This project contains the work done during the course on Database Systems at Saarland University in the Winter Semester 2022-2023.

The skeletal framework for the project, including the build toold and unit tests have already been provided by the course organisers. This also includes the Mutable API ([https://bigdata.uni-saarland.de/teaching/dbsys20/api/](https://bigdata.uni-saarland.de/teaching/dbsys22/api)) for working with the Database System. Our own work here involves actually implementing the concepts stated below in the respective source files.
To build the project, the requirements include e CMake3 3.18 or newer, a C/C++ compiler supporting C++20
(recommended Clang4 or GCC5), and a build automation tool (e.g. GNU Make6 or Ninja7). Source files are located src/ in and files for unit testing are found in unittest/.

This project implements 3 important concepts of a database system:

1. **Row Storage Layout:** 
In the main memory database store, the row layout maps how the relation tuples are physically stored on the storage.

2. **B+ Tree:** 
This section contains the general data structure for a B+ Tree with functionalities such as getters and setters, iterators, lookup, and bulk loading.

3. **Query Optimiser:** 
Implemented an algorithm for cost-based query optimization. The code is divided into three components: a table to track the optimal plan for each subproblem, a cost function to estimate plan costs, and an algorithm to enumerate all feasible plans.

