# Deckard
[![Build Status](https://circleci.com/gh/robolectric/deckard-gradle233.svg?style=svg)](https://circleci.com/gh/robolectric/deckard-gradle233)

A copy of the [Deckard](http://github.com/robolectric/deckard-gradle233) that
uses the Gradle 2.3 plugin. 

It is intended to verify that the latest Robolectric still works with the older
build chain. 

## Setup

*Note: These instructions assume you have a Java 1.8 [JDK](http://www.oracle.com/technetwork/java/javase/downloads/index.html) installed.*

To start a new Android project:

1. Install [Android Studio 2.3](http://developer.android.com/sdk/index.html).
1. Download Deckard as a zip [here](https://github.com/robolectric/deckard-gradle233/archive/master.zip) and then extract it on your dev machine.

1. Import the template into Android Studio by clicking "Import project" and selecting the project directory.

1. Change the names of things from 'Deckard' to whatever is appropriate for your project. Package name, classes, build.gradle, and the AndroidManifest are good places to start.
1. Build an app. Win.

### Running on the command line

1. In the project directory you should be able to run the Robolectric tests:
    ```bash
    ./gradlew test
    ```

1. You can also run the Espresso tests:
    ```bash
    ./gradlew connectedAndroidTest
    ```
    Note: Make sure to start an Emulator or connect a device first so the test has something to connect to.

1. Finally you can build a debug `.apk` of the project for installation on phones:
    ```bash
    ./gradlew assemble
    ```
    This will output the file to `build/outputs/apk/*-debug.apk`
