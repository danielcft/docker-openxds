# docker-openxds
A docker image for the [openxds] project.

## Features
-   Based on the last known version of openxds 1.0.1 *(09/14/2010)*
-   Adds some manual dependencies, inspired by [jembi/openxds]

### Background
Openxds hasn't received any updates in the recent years. 
 The project in the svn repository has broken dependencies, which makes the task of building it cumbersome. 
 
 This docker image should make it easier to build it without these problems.
### Instructions
Build the docker image 

```sh
$ docker build -t docker-openxds .
```

Run the container
```sh
$ docker run docker-openxds
```

This generates a jar file `build/openxds-1.0.1.jar`. If you wish to run the jar inside the container,
```sh
$ docker run docker-openxds -it 
root@container:  cd /build/ && java-jar openxds-1.0.1.jar
```


License
----
MIT

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [jembi/openxds]: <https://github.com/jembi/openxds>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [openxds]: <https://www.projects.openhealthtools.org/sf/projects/openxds/>
   [abandonware]: <https://en.wikipedia.org/wiki/Abandonware>

