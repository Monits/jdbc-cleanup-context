jdbc-cleanup-context
====================

A general purpose context listener to cleanup jdbc drivers and threads to prevent memory leaks.

# Adding the dependency

We use [Maven](http://maven.apache.org/) for building & distributing. You're welcome to use our Maven repositories, or build your own .jar.

To use our Maven repos just add:

    <repositories>
        <repository>
            <id>monits-snapshots</id>
            <url>http://nexus.monits.com/content/repositories/oss-snapshots/</url>
            <name>Monits Snapshots</name>
        </repository>
    </repositories>

    <dependencies>
        <dependency>
            <groupId>com.monits</groupId>
            <artifactId>jdbc-cleanup-context</artifactId>
            <version>1.0-SNAPSHOT</version>
        </dependency>
    </dependencies>

To build a .jar from source:

>
> mvn clean install
>

# Using 

To add the cleaner to your Java web project, just add these lines to your `web.xml`:

    <listener>
        <listener-class>
            com.monits.listener.JDBCCleanupContextListener
        </listener-class>
    </listener>

# Copyright and License

Copyright 2014 Monits.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this work except in compliance with the License. You may obtain a copy of the License at: 

http://www.apache.org/licenses/LICENSE-2.0

