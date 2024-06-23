# Java Application Components

This document provides a hierarchical representation of the components involved in developing and running a Java application.

## Java Application (Source Code)
This is your Java source code, typically in `.java` files.

### JDK (Java Development Kit)
The JDK is essential for Java development and includes the following components:

- **javac (Compiler)**: Converts Java source code into bytecode (`.class` files).
- **JRE (Java Runtime Environment)**: Provides the necessary libraries and JVM for running Java applications.

### JRE (Java Runtime Environment)
The JRE is included within the JDK and contains:

- **Libraries**: Standard libraries needed to run Java applications.
- **JVM (Java Virtual Machine)**: The runtime engine that executes the bytecode.

### JVM (Java Virtual Machine)
The JVM is responsible for running the Java bytecode and includes several critical components:

- **Execution Engine**: Executes the bytecode.
- **Class Loader**: Loads class files.
- **Bytecode Verifier**: Ensures bytecode is valid and secure to run.

This hierarchical representation shows how each component builds upon the previous one to provide a complete environment for developing and running Java applications.


Here's a diagram to illustrate these differences:

```plaintext
+----------------------+
|     Java Application |
|      (Source Code)   |
+----------+-----------+
           |
           v
+----------+-----------+
|    JDK (Java Development Kit)   |
|  +---------+  +-----------------+|
|  | javac   |  | JRE             ||
|  | (Compiler) |                 ||
|  +---------+  +-----------------+|
|              |  +-------------+  ||
|              |  | JVM         |  ||
|              |  +-------------+  ||
|              |                 |  ||
|              +-----------------+  |
+------------------------------------+

           |
           v
+----------+-----------+
|    JRE (Java Runtime Environment)   |
|  +-----------------+                |
|  | Libraries       |                |
|  +-----------------+                |
|  | JVM (Java Virtual Machine)       |
|  +-----------------+                |
+--------------------------------------+

           |
           v
+----------+-----------+
|    JVM (Java Virtual Machine)       |
|  +-----------------+                |
|  | Execution Engine|                |
|  | Class Loader    |                |
|  | Bytecode Verifier|               |
|  +-----------------+                |
+--------------------------------------+



