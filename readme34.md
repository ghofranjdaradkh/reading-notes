Publishing is the general process that makes your Android app available to users. When you publish an Android app, you do the following:

Prepare the app for release.

During the preparation step, you build a release version of your app.

Release the app to users.

During the release step, you publicize, sell, and distribute the release version of your app, which users can download and install on their Android-powered devices.




releases and versioning are closely related in the process of preparing and publishing Android apps. Versioning involves assigning unique version numbers to different releases of an app, typically indicating the level of changes made. Releases represent specific versions of an application that are made available to users. Each release is associated with a unique version number, and the preparation for release includes configuring, testing, updating resources, and ensuring compatibility before distributing the app to users.

Main Tasks to Prepare Your Application for Release to Google Play Store:

Configure Your App for Release:

Disable and remove logging.
Set debuggable to false for Groovy or isDebuggable to false for Kotlin script.
Update the app's version information.

Build and Sign a Release Version:

Use Gradle build files with the release build type to build and sign the release version of your app.

Test the Release Version:

Thoroughly test the release version on target handset and tablet devices.
Consider using Firebase Test Lab for testing across a variety of devices and configurations.

Update App Resources for Release:

Ensure all app resources, such as multimedia files and graphics, are updated and included in the release.

Prepare Remote Servers and Services:

If your app depends on external servers or services, ensure they are secure and production-ready.