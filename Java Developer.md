# Install JDK and Maven

## Install OpenJdk with Brew
- Check specify version: https://formulae.brew.sh/formula/openjdk@11
```bash
brew install openjdk@11
```
## Download & Install Maven
- https://maven.apache.org/download.cgi

## Config 
  
    #vim ~/.zshrc
    
    # Java
      export JAVA_8_HOME=$(/usr/libexec/java_home -v 1.8.0_292)
      export JAVA_11_HOME=$(/usr/libexec/java_home -v 11)
      alias java8='export JAVA_HOME=$JAVA_8_HOME'
      alias java11='export JAVA_HOME=$JAVA_11_HOME'
    # Deafault java version
    java11
    
    # Maven
    export MAVEN_HOME=$HOME/apache-maven-3.8.6
    export PATH=$MAVEN_HOME/bin:$PATH
