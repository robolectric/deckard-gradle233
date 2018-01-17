# Deckard
[![Build Status](https://circleci.com/gh/robolectric/deckard-gradle233.svg?style=svg)](https://circleci.com/gh/robolectric/deckard-gradle233)

Deckard is the simplest possible Java Android application project that uses Robolectric/Espresso for testing and Gradle to build. It has one Activity, a single Robolectric test of that Activity, and an Espresso test of that Activity.

Deckard imports easily into the latest editions of Android Studio with minimal setup.

*Note: A Kotlin variant of this template is also available [here](https://github.com/seadowg/deckard-kotlin).*

## Setup

*Note: These instructions assume you have a Java 1.8 [JDK](http://www.oracle.com/technetwork/java/javase/downloads/index.html) installed.*

To start a new Android project:

1. Install [Android Studio 2.3](http://developer.android.com/sdk/index.html).
1. Download Deckard as a zip [here](https://github.com/robolectric/deckard/archive/master.zip) and then extract it on your dev machine.

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
