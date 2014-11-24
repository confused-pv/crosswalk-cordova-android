# crosswalk-cordova-android

This command line tool is an easy way to migrate your existing Cordova based (including Ionic) projects over to use Crosswalks Chromium webveiw. The performance benefit is huge, you get access to all the latest web APIs, and the only major draw back is increased apk size.

Note : Supports only ARM architecture.
### Version
0.1.1

### Installation

You need Cordova and all of it's dependencies installed globally:

```sh
$ npm i -g crosswalk-cordova-android
```

### Usage

Simply enter your projects root folder and run:

```sh
$ crosswalk-cordova-android
```

This command defaults to Crosswalks 'stable' Cordova Android release and automatically finds your Android SDK target using the `android list` command and some regex magic. Crosswalk also offers 'beta' and 'canary' releases if you'd like to change that or the Android SDK target use these flags:

URL VERSIONS :

stable : supports cordova 3.5, crosswalk 8.37.189.14
beta : supports cordova 3.6.3, crosswalk 10.39.235.6
```sh
$ crosswalk-cordova-android --release beta --target android-19
```

or

```sh
$ crosswalk-cordova-android -r canary -t android-19
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
