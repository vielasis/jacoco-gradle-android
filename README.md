# JaCoCo for Android Projects

A Gradle script that enables you to use JaCoCo for your Android projects. This is tested to work on AGT 4.0.0 and Gradle 6.1.1. No need for third-party plugins!

# Usage
You can download `jacoco.gradle` and place it in your project and apply the plugin as usual
**OR**
just use the raw URL directly:
```
apply from: 'https://raw.githubusercontent.com/vielasis/jacoco-gradle-android/master/jacoco.gradle'
```

# Tasks
The JaCoCo tasks are just your usual unit test tasks suffixed with `Coverage`. i.e. if you just have `debug` and `release` - this will generate `testDebugUnitTestCoverage` and `testReleaseUnitTestCoverage`. The reports are generated in `builds/jacoco` folder.

In general:
`test{variantName}UnitTestCoverage` is the Gradle task generated by this script