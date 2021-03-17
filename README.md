# gradle
Gradle commands and concepts

[Gradle Build Tool](https://gradle.org/)

## setup gradle at linux
```
wget https://services.gradle.org/distributions/gradle-6.8.3-bin.zip

unzip -d /opt/gradle gradle-6.8.3-bin.zip

export GRADLE_HOME=/opt/gradle/gradle-6.8.3-bin

export PATH=$PATH:$GRADLE_HOME/bin
```
## projeto gradle
```
gradle init
```

## edit build.gradle file
```
apply plugin: 'java'

compileJava {
    options.incremental = true
    options.fork = true
    options.failOnError = false
}

compileJava {
    options.release = 8
}

jar {
  manifest {
    attributes 'Main-Class': 'HelloWorld'
  }
}
```

```
gradle tasks
```

```
gradle clean build
```

```
gradle -q <TASK_NAME>
```