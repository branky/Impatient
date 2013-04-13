## Cascading for the Impatient

Welcome to [Cascading for the Impatient](http://www.cascading.org/category/impatient/), a series of blog posts and [Cascading 2.0](http://www.cascading.org/) code examples to get you started. Quickly. Like, yesterday.

This set of progressive coding examples starts with a simple file copy and builds up to a MapReduce implementation of the TF-IDF algorithm.

For more detailed information, please see https://github.com/Cascading/Impatient/wiki

### Part 1
* Implements simplest Cascading app possible
* Copies each TSV line from source tap to sink tap
* Roughly, in about a dozen lines of code
* Physical plan: 1 Mapper

### Part 2
* Implements a simple example of WordCount
* Uses a regex to split the input text lines into a token stream
* Generates a DOT file, to show the Cascading flow graphically
* Physical plan: 1 Mapper, 1 Reducer

### Part 3
* Uses a custom Function to scrub the token stream
* Discusses when to use standard Operations vs. creating custom ones
* Physical plan: 1 Mapper, 1 Reducer

### Part 4
* Shows how to use a HashJoin on two pipes
* Filters a list of stop words out of the token stream
* Physical plan: 1 Mapper, 1 Reducer

### Part 5
* Calculates TF-IDF using an ExpressionFunction
* Shows how to use a CountBy, SumBy, and a CoGroup
* Physical plan: 10 Mappers, 8 Reducers

### Part 6
* Includes unit tests in the build
* Shows how to use other TDD features: checkpoints, assertions, traps, debug
* Physical plan: 11 Mappers, 8 Reducers

### Part 7
* Implements switch to run the example in local mode (without Apache Hadoop)
* Uses an R script to analyze/visualize the results

### Part 8
* Scalding equivalents of previous examples in Cascading
