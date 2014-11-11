# cordova-android-crosswalk

This command line tool is an easy way to migrate your existing Cordova based (including Ionic) projects over to use Crosswalks Chromium webveiw. The performance benefit is huge, you get access to all the latest web APIs, and the only major draw back is increased apk size.

### Version
0.1.1

### Installation

You need Cordova and all of it's dependencies installed globally:

```sh
$ npm i -g cordova-android-crosswalk
```

### Usage

Simply enter your projects root folder and run:

```sh
$ cordova-android-crosswalk
```

This command defaults to Crosswalks 'stable' Cordova Android release and automatically finds your Android SDK target using the `android list` command and some regex magic. Crosswalk also offers 'beta' and 'canary' releases if you'd like to change that or the Android SDK target use these flags:

```sh
$ cordova-android-crosswalk --release canary --target android-18
```

or

```sh
$ cordova-android-crosswalk -r canary -t android-18
```

### Todo's

 - Write Tests
 - Pressure crosswalk-project.org to offer a latest-release url for each build
 - Implement promises to clean up code
 - Add help flag that prints commands
 - Implement more helpful errors

License
----

MIT


**Free Software, Hell Yeah!**
