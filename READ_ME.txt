
SAMPLE GIT HUB https://github.com/firebase/quickstart-android/tree/master/messaging/app/src/main
CLOUD MESSAGING TOPIC https://firebase.google.com/docs/cloud-messaging/android/topic-messaging
APP .GRADLE
######################333
    defaultConfig {
        applicationId "guy.droid.com.firebasepush"
        minSdkVersion 16
        targetSdkVersion 24
        versionCode 1
        versionName "1.0"
        multiDexEnabled true // should be done to run multidex
    }

dependencies {
    compile fileTree(include: ['*.jar'], dir: 'libs')
    testCompile 'junit:junit:4.12'
    compile 'com.android.support:appcompat-v7:24.2.0'
    compile 'com.google.firebase:firebase-core:9.4.0'
    compile 'com.google.android.gms:play-services:9.4.0'
    compile 'com.android.support:multidex:1.0.1'  // allow multidex for playservices above 9.4.0
}
apply plugin: 'com.google.gms.google-services' //add at end

gradle properties 
################################
org.gradle.jvmargs=-Xmx2512M // should write for increase heap size

build.gradle 
#############################
 dependencies {
        classpath 'com.android.tools.build:gradle:2.1.3'
        classpath 'com.google.gms:google-services:3.0.0' // should add to support 9.4.0 pLAY SERVICES
        // NOTE: Do not place your application dependencies here; they belong
        // in the individual module build.gradle files
    }