# How to Set up a Local Java Development Environment

Setting up a development environment for Java can be daunting, so let’s demystify it.

To start with, you will need a few tools:

```bash
-  A Java distribution — This contains all the tools you need to turn Java source code into a program that you can run on your computer. You can’t develop Java applications without this.
-  A build tool — Build tools help you add other libraries to your project and can build and run your application. You could do all that by hand, but a build tool will save you so much time and confusion that we don’t recommend developing without one.
-  An IDE — You can write Java code in any text editor, but a good Integrated Development Environment (IDE) will provide a lot of help: syntax highlighting, refactoring assistance, integration with your build tool, and more.
```
# Installation

An excellent way to install the Java distribution and build tool is with SDKMAN!. After you have installed SDKMAN! — see the above link — you can use the sdk command to install different tools, and different versions of the SDK and Java.

## Install a Java distribution

In a terminal, you can see what versions of Java are available to install using the command sdk list java — there are many, and if you don’t know which you want then we recommend picking the latest HotSpot version from AdoptOpenJDK. New versions are released frequently. At the moment the latest is 15.0.1.hs-adpt (hs is short for HotSpot, adpt for AdoptOpenJDK), so install with:

```bash
sdk install java 15.0.1.hs-adpt
```

This will download the Java distribution and set up any necessary environment variables to use it.

If you aren’t using SDKMAN!, you can download Java directly from AdoptOpenJDK, but you will need to set the JAVA_HOME environment variable yourself as well as making sure that the java command is on your $PATH.

You can check if everything is working correctly by running java -version in a terminal. You should see output like this:

```bash
openjdk version "15.0.1" 2020-10-20
OpenJDK Runtime Environment AdoptOpenJDK (build 15.0.1+9)
OpenJDK 64-Bit Server VM AdoptOpenJDK (build 15.0.1+9, mixed mode, sharing)
```

## Install a build tool

The two most popular build tools are Maven and Gradle. Maven is more widely used so if you are not sure which to choose, we recommend installing that.

To install Maven with SDKMAN!, type the following command:

```bash
sdk install maven 3.6.3
```

Without SDKMAN!, you will need to download and install it yourself.

Check if Maven is installed correctly with mvn --version. It should print something like the this:

```bash
Apache Maven 3.6.3 (cecedd343002696d0abb50b32b541b8a6ba2883f)
Maven home: /home/twilio/.sdkman/candidates/maven/current
Java version: 15.0.1, vendor: AdoptOpenJDK, runtime: /home/twilio/.sdkman/candidates/java/15.0.1.hs-adpt
Default locale: en_GB, platform encoding: UTF-8
OS name: "linux", version: "5.3.0-53-generic", arch: "amd64", family: "unix"
```

## Install an IDE
The most popular IDE for Java is Intellij IDEA. The community edition is free and very powerful. There are other IDEs — if you are familiar with Eclipse or Netbeans then feel free to use them too. There is also good Java support in Microsoft Visual Studio Code.

After downloading and installing an IDE, you are ready to create Java applications.

# Create a Java project

With your IDE, create a new project and then select Maven or Gradle as the build tool. This will create the correct directory structure and open the project. For either build tool, your application’s source code will go in src/main/java.

To check that everything is working correctly, create a file called HelloTwilio.java in src/main/java with the following contents:
```bash
public class HelloTwilio {
  public static void main(String[] args) {
    System.out.println("Hello Twilio");
  }
}
```
# Create A Twilio Application
https://www.twilio.com/docs/usage/quickstart/devenvironment-java#create-a-twilio-application
