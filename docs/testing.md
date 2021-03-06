# Testing

The functionality and user interface of the program has been tested on a linux environment manually. 
The application logic of program has also been tested on a unit and integration level with automated JUnit tests.

## Unit Testing 
Individual methods of each essential class in the program is tested by a separate JUnit test class. For example, the markovManager class is tested by a markovManagerTest class, and so on. The only classes that were not tested wre the markovUI class and the SimDao interface. 
the SimFromFile class has the SimFromFileTest class and so on. The data-access functionality of the class SimFromFile is tested with temporary files, and database class is tested on a test database.

## Integration Testing
The tests in the testing classes include tests that combine functionality from different classes. There are no special classes used for integration testing.
Some level of integration testing was of course conducted manually. 

## Test Coverage
The automated testing covers 94 % of all instructions and 82% of branches. The user interface is excluded. Below is a screenshot of the report
generated by Jacoco.

![pic](/docs/pictures/testikattavuus.png)

## Manual testing

The functionality of the program was also tested manually on a Linux environment. The testing included giving incorrect inputs such as filenames, 
node descriptors, empty inputs and pre-existing connections between nodes.  

## Gaps in Testing

The program has not been tested in a MacOS environment. The automated unit tests also do not cover all the methods of the classes
individually, even though many of them are covered by integration testing. For example, there is no unit test for the save method of the 
SimFromDb class.
