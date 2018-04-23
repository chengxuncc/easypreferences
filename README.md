<h1 align="center">Android Shared Preferences</h1>
<p align="center">
  <a href="https://jitpack.io/#mukeshsolanki/Android-Shared-Preferences-TinyDB-"><img src="https://jitpack.io/v/mukeshsolanki/Android-Shared-Preferences-TinyDB-/month.svg"/></a>
  <a href="https://android-arsenal.com/api?level=9"> <img src="https://img.shields.io/badge/API-9%2B-blue.svg?style=flat" /></a>
  <a href="https://jitpack.io/#mukeshsolanki/Android-Shared-Preferences-TinyDB-"> <img src="https://jitpack.io/v/mukeshsolanki/Android-Shared-Preferences-TinyDB-.svg" /></a>
  <a href="http://android-arsenal.com/details/1/3805"> <img src="https://img.shields.io/badge/Android%20Arsenal-Android--Shared--Preferences-brightgreen.svg?style=flat" /></a>
  <a href="https://travis-ci.org/mukeshsolanki/Android-Shared-Preferences-TinyDB-"> <img src="https://travis-ci.org/mukeshsolanki/Android-Shared-Preferences-TinyDB-.svg?branch=master" /></a>
  <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg"/></a>
  <a href="https://www.paypal.me/mukeshsolanki"> <img src="https://img.shields.io/badge/paypal-donate-yellow.svg" /></a>
  <br /><br />
  A simple easy to use library that helps you quickly store and retrive data from shared preferences
</p>

## How to integrate into your app?

Integrating the library into you app is extremely easy. A few changes in the build gradle and your all ready to use TinyDB. Make the following changes.

Step 1. Add the JitPack repository to your build file. Add it in your root build.gradle at the end of repositories:

```java
allprojects {
  repositories {
    ...
    maven { url "https://jitpack.io" }
  }
}
```
Step 2. Add the dependency
```java
dependencies {
        implementation 'com.github.mukeshsolanki:easypreferences:<latest-version>'
}
```

## How to use the library?
Okay seems like you integrated the library in your project but **how do you use it**? Well its really easy just follow the steps below.

```
 //Create a new instance of TinyDB
 EasyPrefrences easyPrefrences=new EasyPrefrences(appContext);
 
 //use that instance to save data
 
 easyPrefrences.putString(key,value); //Save's a string value in your preferences
 easyPrefrences.putInt(key,value); //Save's a int value in your preferences
 
 
 //use that instance to retrieve data
 easyPrefrences.getString(key); //retrives the data from preferences or default values if it does not exists
 easyPrefrences.getBoolean(key); //retrives the data from preferences or default values if it does not exists
```
That's pretty much it. Looks like your all done here.

## Author
Maintained by [Mukesh Solanki](https://www.github.com/mukeshsolanki)

## Contribution
[![GitHub contributors](https://img.shields.io/github/contributors/mukeshsolanki/easypreferences.svg)](https://github.com/mukeshsolanki/easypreferences/graphs/contributors)

* Bug reports and pull requests are welcome.
* Make sure you use [square/java-code-styles](https://github.com/square/java-code-styles) to format your code.

## License
```
Copyright 2018 Mukesh Solanki

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```