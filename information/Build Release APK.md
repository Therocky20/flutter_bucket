[**WEB SITE**](https://flutter.dev/docs/deployment/android)
# Review the App Manifest
1. Same in the website
# Review the build configuration
1. Same in the website
# Adding a Launcher icon
1. Similar in the website but only replace flutter icon (ic_launcher.png)
# Create a keystore
1.	open the cmd in the java bin folder (for example: C:\Program Files\Java\jdk1.8.0_201\bin or AndroidStudio/jre/bin)
2.	Execute: keytool -genkey -v -keystore <DESTINATION_PATH>key.jks -keyalg RSA -keysize 2048 -validity 10000 -alias key
* The DESTINATION_PATH is raccomanded the same project directory
# Reference the keystore from the app
1.	Same in the website
2.	Add in.. (OPTIONAL: why add this code? More information in https://medium.com/flutterpub/flutter-app-couldnt-find-libflutter-so-c95ad81cbccd )
`android {
     ...
     defaultConfig {
         ...`
3. Add this code:
`ndk {
     abiFilters 'armeabi-v7a'
 }`
# Building a release APK
1. Same in the website