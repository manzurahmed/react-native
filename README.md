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

It takes almost **1 Hour** to download Android SDK Tools, Android SDK Platform-Tools, Emulator, Build Tools, Haxm, Platform, etc. over 2Mbps connection.

Unfortunately, I had a Core2Duo PC which does not support Hardware Virtualization. As a result, I got the following error messages,

```
Unable to install Intel HAXM
Your CPU does not support VT-x.
Unfortunately, your computer does not support hardware accelerated virtualization.
Here are some of your options:
 1) Use a physical device for testing
 2) Develop on a Windows/OSX computer with an Intel processor that supports VT-x and NX
 3) Develop on a Linux computer that supports VT-x or SVM
 4) Use an Android Virtual Device based on an ARM system image
   (This is 10x slower than hardware accelerated virtualization)
```

## Create Virtual Device

- Click on "Tools" -> "ADM Manager" and click on "+Create Virtual Device".
- A form will appear. Select "Next 2" having screen size of 5 inches.
- Click Next.
- "System Image" screen will appear. I selected "Nougat" to download and install it. "Nougat" system image is 928 MB and takes about 1 hour and 30 minutes to download over 2Mbps Internet connection.

Let Android Studio download and complete the component installation.

When Nougat installation finishes, select it and Press "Next".
On the next screen, "Verify Configuration, keep every thing unchanged as prescribed by Android Studio and press "Finish".

[Create New Device](https://github.com/manzurahmed/react-native/blob/master/create_new_device.jpg)
