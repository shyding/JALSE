## JALSE - Java Artificial Life Simulation Engine
[![Build Status](https://travis-ci.org/Ellzord/JALSE.svg?branch=master)](https://travis-ci.org/Ellzord/JALSE)
[![Coverage Status](https://coveralls.io/repos/Ellzord/JALSE/badge.svg?branch=master)](https://coveralls.io/r/Ellzord/JALSE?branch=master)
[![Maven Central](https://maven-badges.herokuapp.com/maven-central/com.github.ellzord/JALSE/badge.svg)](https://maven-badges.herokuapp.com/maven-central/com.github.ellzord/JALSE/)
[![License](http://img.shields.io/:license-apache-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)

JALSE is a lightweight entity framework for simulation written in Java 8. The framework is used to create a dynamic living data-model for your entity based simulation or game. By default all JALSE enitites can have their attributes and child entities concurrently processed and mutated (no need for additional synchronisation).

JALSE takes entities one step further by allowing the user to create Entity types. Unlike classic Java objects JALSE entities can have multiple types and 'casting' to another type causes no issues (just null fields). As well as making use of type erasure (```assert cowEntity.isMooing();```) entities can be grouped and processed by entity type. Inheritence still is at play here so I can be sure to move all ```Animal```s but only ```moo()`` the cows!

Use JALSE for when you need to start processing entities in the thousands or if you want a structured way to increase the level of detail kept about an entity (cant just add fields forever).

Founded by [Elliot Ford](https://twitter.com/ellzord)

### Documentation
See the [Wiki](https://github.com/Ellzord/JALSE/wiki) for full documentation, examples and project information.

See the [API docs](http://ellzord.github.io/JALSE/docs/).

### Getting the latest release
JALSE [releases](https://github.com/Ellzord/JALSE/releases) and (SNAPSHOTS) are published to maven central (http://search.maven.org/).

Example for Maven:
```xml
<dependency>
    <groupId>com.github.ellzord</groupId>
    <artifactId>JALSE</artifactId>
    <version>1.0.4</version>
</dependency>
```

Example for Gradle:
```
compile 'com.github.ellzord:JALSE:1.0.4'
```

### Links
* [Example projects](https://github.com/Ellzord/JALSE/wiki/Example-projects)
* [Code snippets](https://github.com/Ellzord/JALSE/wiki/Code-snippets)
* [How to contribute](https://github.com/Ellzord/JALSE/wiki/How-to-contribute)
* [Have bugs or questions?](https://github.com/Ellzord/JALSE/wiki/Have-bugs-or-questions%3F)
* [Class diagram](https://github.com/Ellzord/JALSE/wiki/Class-diagram)
* [Technologies we use](https://github.com/Ellzord/JALSE/wiki/Technologies-we-use)
* [Example use cases](https://github.com/Ellzord/JALSE/wiki/Example-use-cases)

### Licence
Code is under the [Apache Licence v2](http://www.apache.org/licenses/LICENSE-2.0.html).
