cherimojava-parent [![Build Status](https://travis-ci.org/cherimojava/cherimojava-parent.png?branch=master)](https://travis-ci.org/cherimojava/cherimojava-parent)
===========
Base maven parent for cherimojava based artifacts, providing a common version stack of artifacts and plugins. Each artifact for cherimojava should use this as parent pom.
POM file is semantic versioned in this way:

* Major will be updated if the pom is updated for new java releases. So once the code compatibility is raised from Java 8 to Java 9. The pom file version will move from 1 to 2. The same happens for future code compatibility changes.
* Minor will be updated if artifacts referenced are changing in a way that the compatibility is affected.
* Patch wil be updated for minor changes like new artifacts referenced and dependency changes of these, only affecting bug-fixes and backward compatible changes

Maven dependency
------
    <dependency>
        <groupId>com.github.cherimojava</groupId>
        <artifactId>parent</artifactId>
        <version>1.0.0-SNAPSHOT</version>
    </dependency>
