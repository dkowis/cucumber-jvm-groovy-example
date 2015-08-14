A sample cucumber-jvm groovy project built using gradle!

[![Build Status](https://travis-ci.org/dkowis/cucumber-jvm-groovy-example.svg?branch=master)](https://travis-ci.org/dkowis/cucumber-jvm-groovy-example)

### Versions
 * Gradle: 1.7 
 * Cucumber-jvm: as listed in the build.gradle file!

### Instructions
To build the project you can follow standard gradle build stuffs.

I've added a custom cucumber task necessary to run the Cucumber CLI against the groovy scripts and the feature files.

```gradle cucumber```

to run that and you should then have a nice pretty green (for the most part) output from gradle as the cucumber features
are executed. It'd be easy enough to glue the cucumber task to happen as part of the testing cycle or before a deployment.

### NOTE

You can't run `gradle test`. It's XML output mechanism that it uses for executing the Junit tests doesn't like to make files
named 'Scenario: Regular Numbers.xml'. Easy to overcome using the `gradle cucumber` task, and probably a "bug" in gradle,
but I'm not yet bothered to bug them about it.
