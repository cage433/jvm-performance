A simple performance testing framework
-------------------------------------

Created as http://scalameter.github.io/ appears to no longer be active

Requirements
------------
- Creating a new Suite should require no more than instantiating a trait
- Tests should be runnable from the command line, either 'all tests in classpath'
  or 'named test(s)'
- History of results should be kept, using a Kolmogorov-Smirnov test to check for 
  regression
- Tests should specify how large a heap to be used, and any other JVM parameters
- Tests should specify numbers of warm-up runs and actual runs
- Tests should optionally be able to exclude runs in which a full GC occurred

Later requirements
------------------

Not needed initially, but nice to have
- Results should be graphable against git commit
- Numbers of GCs should be reported, and optionally cause a test to fail if there
  are too many.
- Should be easy to use 'git bisect' to find regressions
