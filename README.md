# cordova-android-crosswalk

This command line tool is an easy way to migrate your existing Cordova based (including Ionic) projects over to use Crosswalks Chromium webview. The performance benefit is huge, you get access to all the latest web APIs, and the only major draw back is increased apk size.

### Version
0.3.6

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

Use `-r` or `--release` to specify Crosswalk release channel. Three
possible choices "canary", "beta", or "stable". Defaults to "stable".

```sh
$ cordova-android-crosswalk -r canary
```

Use `-t` or `--target` to specify the target android version. Defaults to
highest target version from `android list target -c`.

```sh
$ cordova-android-crosswalk -t android-21
```

Use `-p` or `--preserve` to maintain your prexisting Crosswalk bundle download.
Default downloads Crosswalk everytime.

```sh
$ cordova-android-crosswalk -p
```

Use `-x` or `--xwalk-version` to specify Crosswalk release version. Defaults
to latest stable version.

```sh
$ cordova-android-crosswalk -x 9.38.208.10
```
Use `-a` or `--arch` to choose between arm and x86 architectures. Two possible
chioces "x86" or "arm". Defaults to both.

```sh
$ cordova-android-crosswalk -a x86
```

Use `-f` or `--force` to suppress build warnings.

```sh
$ cordova-android-crosswalk -f
```

Use `-h` or `--help` prints list of flags.

```sh
$ cordova-android-crosswalk -h
```

Use `-v` or `--version` prints cordova-android-crosswalk version.

```sh
$ cordova-android-crosswalk -v
```



### Todo's

 - Write Tests
 - ~~Add Cordova version check for 3.5~~
 - Pressure crosswalk-project.org to offer a latest-release url for each build
 - ~~Implement promises to clean up code~~
 - ~~Add help flag that prints commands~~
 - ~~Add version flag~~
 - ~~Implement more helpful errors~~

License
----

MIT


**Free Software, Hell Yeah!**

[migration guide]:https://crosswalk-project.org/documentation/cordova/migrate_an_application.html