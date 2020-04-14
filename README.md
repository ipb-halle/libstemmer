= Mavenized Snowball Stemmer = 
This project brings the Snowball stemmer [](https://snowballstem.org/) 
to your local Maven cache. Just clone this project and install it:

    git clone ...
    mvn install

The build process downloads the current `libstemmer_java.tgz` from GitHub, 
extracts it, compiles, tests, packages, and finally installs the jar in 
your local maven cache. 

You can then use the snowball stemmer by including 

  <dependency>
    <groupId>org.tartarus</groupId>
    <artifactId>snowball</artifactId> 
    <version>2.0.0</version>
  </dependency>

in your `pom.xml`. 

**Note:** The artifact will be only available locally; there is currently no 
deployment to central repositories (Maven Central Repository etc.)!

== Licensing ==
This code is released under the same BSD-3-Clause license as the snowball stemmer code
[](https://github.com/snowballstem/snowball)
