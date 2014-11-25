# cordova-android-crosswalk

This command line tool is an easy way to migrate your existing Cordova based (including Ionic) projects over to use Crosswalks Chromium webview. The performance benefit is huge, you get access to all the latest web APIs, and the only major draw back is increased apk size.

##### Caution!
Please use Cordova 3.5 for initially building and running your projects. Crosswalk
currently works with Cordova 3.5 only. You can install using `$ npm install -g cordova@3.5`.
See more details on Crosswalks official [migration guide].

### Version
0.1.2

### Installation

You need Cordova and all of it's dependencies installed globally:

```sh
$ npm install -g cordova-android-crosswalk
```

### Usage

Simply enter your projects root folder and run:

```sh
$ cordova-android-crosswalk
```

This command defaults to Crosswalks 'stable' Cordova Android release and automatically finds your Android SDK target using the `$ android list` command and some regex magic. Crosswalk also offers 'beta' and 'canary' releases if you'd like to change that or the Android SDK target use these flags:

```sh
$ cordova-android-crosswalk --release canary --target android-19
```

or

```sh
$ cordova-android-crosswalk -r canary -t android-19
```

### Todo's

 - Write Tests
 - ~~Add Cordova version check for 3.5~~
 - Pressure crosswalk-project.org to offer a latest-release url for each build
 - ~~Implement promises to clean up code~~
 - Add help flag that prints commands
 - ~~Implement more helpful errors~~

License
----

MIT


**Free Software, Hell Yeah!**

[migration guide]:https://crosswalk-project.org/documentation/cordova/migrate_an_application.html