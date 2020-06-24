# Distributed Programming in Java  

These mini projects are programming assignments for Parallel Programming in Java offered by Rice University on Coursera, as a part of [Parallel, Concurrent, and Distributed Programming in Java Specialization](https://www.coursera.org/specializations/pcdp)

Check my repositories of [Parallel Programming in Java](https://github.com/MaiqiDing/Parallel-Programming-in-Java) and [Concurrent Programming in Java](https://github.com/MaiqiDing/Concurrent-Programming-in-Java). 

## Compiling  
### Compiling with Maven from Command Line 

`$ mvn compile`

### Compiling with Maven using Intellij

Import project > select miniproject_ directory > Import project from external model, select Maven.

### Compiling Manually using Javac

You will need to add the following JARs to your classpath while building both the provided source and test files using javac

`$ javac -cp ./hamcrest-core-1.3.jar:./junit-4.12.jar:target/classes/:target/test-classes/ src/main/java/edu/coursera/distributed/Setup.java src/test/java/edu/coursera/distributed/SetupTest.java`

## Testing

### Testing with Maven

`$ mvn test`

### Testing with Maven using Intellij

Navigate to View > Tool Windows > Maven. From the Maven Projects pane, expand the Lifecycle section and double-click "test" to automatically run the tests.

### Testing Manually from Command Line

`$ java -cp ./hamcrest-core-1.3.jar:./junit-4.12.jar:target/classes/:target/test-classes/ org.junit.runner.JUnitCore edu.coursera.distributed.SetupTest`

## Contents

### miniproject_1

Implementation of Page Rank algorithm with Spark

Implemented the transformations needed to complete a single iteration of the iterative PageRank algorithm given an input Spark Resilient Distributed Dataset (RDD) of websites.

### miniproject_2

A Simple File Server

Implemented a simple, stripped down file server using Java Sockets that responds to HTTP requests by loading the contents of files and transmitting them to file server clients.

### miniproject_3

Matrix Multiply in MPI

Implemented a method to perform a matrix-matrix multiply in parallel using SPMD parallelism and MPI.

##### MPI Installation

If you would like to test on your local machine, you will need to install an MPI implementation.

Ubuntu, install OpenMPI with the following commands:

`$ sudo apt-get update`

`$ sudo apt-get install -y openmpi-bin libopenmpi-dev`

Linux or Mac OS, download the OpenMPI implementation from:

https://www.open-mpi.org/software/ompi/v2.0/

and following the build instructions in the "User Builds" section of the included INSTALL file. Following installation, you must also add the created OpenMPI bin/ folder to your PATH and the created OpenMPI lib/ folder to your LD_LIBRARY_PATH (on Linux) or your DYLD_LIBRARY_PATH (on Mac OS).

### miniproject_4

Multi-Threaded File Server

Made a simple extension to the file server in miniproject_2 by using multiple Java Threads to handle file requests.

## Author

Maiqi Ding
