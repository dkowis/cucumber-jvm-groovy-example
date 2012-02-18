A sample cucumber-jvm groovy project built using gradle!

### Versions
 * Gradle: 1.0-milestone-8
 * Cucumber-jvm: as listed in the build.gradle file!

### Instructions
To build the project you can follow standard gradle build stuffs.

I've added a custom cucumber task that runs the Cucumber CLI against the groovy scripts and the feature files.

```gradle cucumber```

to run that and you should then have a nice pretty green (for the most part) output from gradle as the cucumber features
are executed. It'd be easy enough to glue the cucumber task to happen as part of the testing cycle or before a deployment.