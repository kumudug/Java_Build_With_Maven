# Java_Build_With_Maven
https://spring.io/guides/gs/maven/

mvn compile

This will run Maven, telling it to execute the compile goal. When it’s finished, you should find the compiled .class files in the target/classes directory.
Since it’s unlikely that you’ll want to distribute or work with .class files directly, you’ll probably want to run the package goal instead:

mvn package


Maven also maintains a repository of dependencies on your local machine (usually in a .m2/repository directory in your home directory) for quick access to project dependencies.
If you’d like to install your project’s JAR file to that local repository, then you should invoke the install goal:

mvn install

The install goal will compile, test, and package your project’s code and then copy it into the local dependency repository,
ready for another project to reference it as a dependency.


mvn test

