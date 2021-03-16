# gradle
Gradle commands and concepts

[Gradle Build Tool](https://gradle.org/)

## projeto gradle
```
gradle init
```

## edit build.gradle file
apply plugin: 'java'
jar {
  manifest {
    attributes 'Main-Class': 'HelloWorld'
  }
}

```
gradle tasks
```

```
gradle build
```

```
gradle -q <TASK_NAME>
```
https://www.youtube.com/watch?v=9wpyYHyTs3c
40:52 de 01:09:50
