# react-native

# Setup Environment on Windows 10

1. Install JDK Windows 64bit (https://www.oracle.com/technetwork/java/javase/downloads/index.html) - 158MB
2. Install NodeJS (https://nodejs.org/en/) - 
3. Install Python (https://www.python.org/downloads/windows/) - 24.4MB
4. Install Android Studio and SDK (https://developer.android.com/studio) - 971MB
5. Command line tools only (https://developer.android.com/studio/index.html#downloads)

**Note:** Android SDK is NOT included in Android Studio .exe installer. AS downloads the SDK on the first run.

**Additional Reading**
- How to install the Android SDK on Windows, Mac and Linux (https://www.androidcentral.com/installing-android-sdk-windows-mac-and-linux-tutorial)
- Android IDE and SDK: How to Install and Get Started (https://www.ntu.edu.sg/home/ehchua/programming/android/android_howto.html)


6. Instal react-native-cli from CMD
```
npm install -g react-native-cli
```

Navigate to "d:\xampp\htdocs" folder and create a new folder, "reactnative" and change to the folder.

```
mkdir reactnative
cd reactnative
```

Now, I am going to create a React Native app by using the following command,
```
react-native init albums
```

## Starting Android Studio on the first time

On the first run, Android Studio tries to import settings from previous installation. Do not import anything.

It starts a Setup Wizard. 

Choose "Standard" as Install Type.
Choose default "Light" theme as "Select UI Theme".
In "Verify Settings" wizard page, Android Studio will download and install Android SDK. Ddefault SDK path is "**C:\Users\<PC-NAME>\AppData\Local\Android\Sdk**".

It takes almost 15 minutes to download the SDK (Android SDK Tools (revision: 26.1.1)) over 2Mbps connection.
