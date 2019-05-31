Android SDK for Dexecure

[ ![Download](https://api.bintray.com/packages/dexecure/maven/android-sdk/images/download.svg?version=0.0.1) ](https://bintray.com/dexecure/maven/android-sdk/0.0.1/link)


A Java client library for generating URLs with dexecure. dexecure is a high-performance distributed image processing service. More information can be found at https://dexassets.dexecure.net/

# Dependencies

The library itself has no external dependencies. Although if you want to build from source (or run tests) then you need ant and the JDK 1.6+.

# Install Options

# Gradle & JCenter
To add Dexecure-Java to your project, include the following in your project's build.gradle:


dependencies {

   compile 'net.dexecure.dexassets:lib:0.0.1'
  
}


And if this is your first external JCenter dependency you'll need to add, again to your project level build.gradle, the following:


buildscript {

    repositories {
    
        google()
        
        jcenter()
        
    }
}

# Running Tests

To run tests clone this project and run:

gradle test

Dependencies for running tests (junit, etc) are provided (in android-sdk/lib/src/androidTest/java/net/dexecure/dexassets/lib/ and referenced in the build config).

# Basic Usage

To begin creating imgix URLs programmatically, simply add the jar to your project's classpath and import the imgix library. The URL builder can be reused to create URLs for any images on the domains it is provided.

