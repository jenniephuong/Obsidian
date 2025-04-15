> more than one class shares data (that is not in the form of a database where the data integrity is protected) e.g. classes sharing a global variable / data structure

why is common coupling bad
- lack of clear responsibility for the data [[Single Responsibility Principle (SRP)]]
- difficult to determine which classes affect a data element making [[Maintenance]] difficult (could accidentally change the value)
- difficult to reuse classes

Fix with [[Replace Magic Number With Symbolic Constant]] refactoring

what is an example of common coupling
- having a data class for airport system storing flight data which gets data from many places, supplies data to many places, many classes can read and write directly to the global data store

#L4_SoftwareComplexity 