# Java SE 17 Advanced Language Features

These examples and exercises are part of the course "Java SE 17 Advanced Language Features" by Jesper de Jong at [Pluralsight](https://www.pluralsight.com/).

## Lambda Expressions and Method References

In this module, you'll learn:

* That lambda expressions are really anonymous methods. 
* What exactly a functional interface is.
* What standard functional interfaces are available in the package `java.util.function`.
* That lambda expressions can capture local variables, which must be effectively final.
* Core principles of the functional programming style.
* That working with checked exceptions in lambda expressions can be cumbersome.
* The four types of method references.

### References

* [Java Language Specification - 15.27 Lambda Expressions](https://docs.oracle.com/javase/specs/jls/se17/html/jls-15.html#jls-15.27)
* [Java Language Specification - 9.8 Functional Interfaces](https://docs.oracle.com/javase/specs/jls/se17/html/jls-9.html#jls-9.8)
* [Java Language Specification - 9.6.4.9 `@FunctionalInterface`](https://docs.oracle.com/javase/specs/jls/se17/html/jls-9.html#jls-9.6.4.9)
* [Java Language Specification - 15.13 Method Reference Expressions](https://docs.oracle.com/javase/specs/jls/se17/html/jls-15.html#jls-15.13)

## Examples

Take a look at the examples from the demos in the course, which you can find in the package: `com.pluralsight.advancedjava.examples`.

## Exercises

To really learn any subject, it's not enough to read a website, book or watch videos. You'll have to work with the subject yourself!

To help you practice there are exercises included, which you can find in the package: `com.pluralsight.advancedjava.exercises`.

To check if you have done the exercises correctly, you can run the included unit tests. You can find the tests in the directory `src/test/java`,
package `com.pluralsight.advancedjava.exercises`.

An IDE such as IntelliJ will make it easy to run the tests: in the Project view (on the left side), right-click one of the test classes and click
"Run 'classname'" from the popup menu.

### Running on the command line

This example project is a [Maven](https://maven.apache.org/) project. Apache Maven is a very widely used project management tool for Java projects.
Most Java IDEs, such as IntelliJ IDEA and Eclipse, understand Maven projects, so it should be easy to open the project in your Java IDE.

If you want or need to work with the project in a terminal window or in the Windows command prompt or PowerShell, then you can use the following commands
to compile the code and run the unit tests. The unit tests will check if you've successfully solved the exercises.

In the terminal, Windows command prompt or PowerShell, first use the `cd` command to go to the directory where you've unzipped this project.
Then use one of the following commands:

On Windows:

    mvnw.cmd clean package

On macOS or Linux:

    ./mvnw clean package

These commands will download Apache Maven if you haven't already have it installed, and then run Maven to compile the code and run the unit tests.

If everything compiles without errors and all the tests succeed, the command will finish with a message that says "BUILD SUCCESS".

To compile the code without running the unit tests, add the `-DskipTests` option:

On Windows:

    mvnw.cmd clean package -DskipTests

On macOS or Linux:

    ./mvnw clean package -DskipTests