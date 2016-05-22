# appendix D Spring Boot dependencies

Whether you’re building your project with Maven or Gradle or you’re working with the Spring Boot CLI, Spring Boot provides dependency management support for several libraries that are commonly used in Spring applications. Table D.1 lists all of the library dependencies supported by Spring Boot version 1.3.0.



```
compile("com.h2database:h2")
```

The same dependency can be declared in a Maven build like this:

```
<dependency>

Notice that in both cases, you shouldn’t need to specify the version. Spring Boot’s dependency management will take care of that for you. You may, however, explicitly provide the version if you want to override the version chosen by Spring Boot.

```
@Grab("h2")
```

When using the @Grab annotation to include any of the libraries in table D.1, you only need to specify the artifact. Spring Boot extends @Grab to infer the group and version for you.

__Table D.1 Library dependencies supported by Spring Boot__

| Group | Artifact | Version |
|-------|----------|---------|