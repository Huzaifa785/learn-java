## Setup Java on your PC step-by-step

### Step 1: Download the JDK

Get it here:- [Java JDK](https://www.oracle.com/in/java/technologies/downloads/)

- The JDK includes tools for developing and testing programs written in the Java programming language and running on the Java platform.
- As of now we'll downloading the JDK 17 version.

### Step 2: Install the JDK

- After downloading the JDK, run the installer.
- Follow the instructions on the screen.
- The JDK is installed in the directory you specified during the installation.

### Step 3: Set the JAVA_HOME environment variable

- The JAVA_HOME environment variable must point to the directory where the JDK is installed.

- To set the JAVA_HOME environment variable on Windows, do the following:

1. Open the Control Panel.
2. Click System.
3. Click Advanced system settings.
4. Click Environment Variables.
5. Under System variables, click New.
6. In the Variable name field, type JAVA_HOME.
7. In the Variable value field, type the directory where the JDK is installed. For example, C:\Program Files\Java\jdk1.8.0_60.
8. Click OK.

- To set the JAVA_HOME environment variable on Linux, do the following:

1. Open a terminal window.
2. Type the following command, where <JDK_install_directory> is the directory where the JDK is installed:

```
export JAVA_HOME=<JDK_install_directory>
```

3. Type the following command to verify that the variable is set correctly:

```
echo $JAVA_HOME
```

- On macOS, the JAVA_HOME environment variable is set by default.

### Step 4: Add the JDK bin directory to the PATH environment variable

- The PATH environment variable must include the bin directory of the JDK.

- To add the JDK bin directory to the PATH environment variable on Windows, do the following:

1. Open the Control Panel.
2. Click System.
3. Click Advanced system settings.
4. Click Environment Variables.
5. Under System variables, click Path, and then click Edit.
6. In the Variable value field, type the following:

```
%JAVA_HOME%\bin
```

7. Click OK.

- To add the JDK bin directory to the PATH environment variable on Linux, do the following:

1. Open a terminal window.
2. Type the following command, where <JDK_install_directory> is the directory where the JDK is installed:

```
export PATH=$PATH:<JDK_install_directory>/bin
```

3. Type the following command to verify that the variable is set correctly:

```
echo $PATH
```

- On macOS, the PATH environment variable is set by default.

### Step 5: Verify the installation

- To verify that the JDK is installed correctly, open a command prompt and type the following command:

```
java -version
```

- If the installation is successful, the following information is displayed:

```
java version "17" 2021-09-14
Java(TM) SE Runtime Environment (build 17+35-2724)
Java HotSpot(TM) 64-Bit Server VM (build 17+35-2724, mixed mode, sharing)
```

- To verify that the PATH environment variable is set correctly, open a command prompt and type the following command:

```
javac -version
```

- If the installation is successful, the following information is displayed:

```
javac 17
```

### Step 6: Install an IDE

- An IDE is a software application that provides comprehensive facilities to computer programmers for software development. An IDE normally consists of a source code editor, build automation tools and a debugger.

- We'll be using [VS Code](https://code.visualstudio.com/) as our IDE.

- Download and install VS Code from [here](https://code.visualstudio.com/).

- After installing VS Code, open it and install the Java Extension Pack.

- To install the Java Extension Pack, click on the Extensions icon on the left side of the screen and search for Java Extension Pack.

- Click on the Install button to install the Java Extension Pack.

- After installing the Java Extension Pack, restart VS Code.

- To verify that the Java Extension Pack is installed correctly, open a new Java file and type the following code:

```
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

- To run the code, click on the Run button on the top right corner of the screen.

- If the installation is successful, the following output is displayed:

```
Hello, World!
```
