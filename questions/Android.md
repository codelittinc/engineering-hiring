# Android


## Basic Questions

- **What do you think are some disadvantages of Android?**  
  Given that Android is an open-source platform, and the fact that different Android operating systems have been released on different mobile devices, there’s no clear cut policy to how applications can adapt with various OS versions and upgrades. One app that runs on this particular version of Android OS may or may not run on another version. Another disadvantage is that since mobile devices such as phones and tabs come in different sizes and forms, it poses a challenge for developers to create apps that can adjust correctly to the right screen size and other varying features and specs.


- **What are the core components under the Android application architecture?**  
  There are 5 key components under the Android application architecture:
  - services
  - intent
  - resource externalization
  - notifications
  - content providers


- **What is the AndroidManifest.xml?**  
  This file is essential in every application. It is declared in the root directory and contains information about the application that the Android system must know before the codes can be executed.


- **Describe Activities**
  Activities are what you refer to as the window to a user interface. Just as you create windows in order to display output or to ask for an input in the form of dialog boxes, activities play the same role, though it may not always be in the form of a user interface.


- **What are Intents?**
  Intents displays notification messages to the user from within the Android enabled device. It can be used to alert the user of a particular state that occurred. Users can be made to respond to intents.

- **Differentiate Activities from Services.**
  Activities can be closed, or terminated anytime the user wishes. On the other hand, services are designed to run behind the scenes, and can act independently. Most services run continuously, regardless of whether there are certain or no activities being executed.


- **What are containers?**
  Containers, as the name itself implies, holds objects and widgets together, depending on which specific items are needed and in what particular arrangement that is wanted. Containers may hold labels, fields, buttons, or even child containers, as examples.

- **What is Orientation?**
Orientation, which can be set using setOrientation(), dictates if the LinearLayout is represented as a row or as a column. Values are set as either HORIZONTAL or VERTICAL.


- **What are the four essential states of an activity?**
  - Active – if the activity is at the foreground
  - Paused – if the activity is at the background and still visible
  - Stopped – if the activity is not visible and therefore is hidden or obscured by another activity
  - Destroyed – when the activity process is killed or completed terminated


- **Name some Android programming languages.**
  - **Java**: One of the most popular programming languages, Java has always been a starting point for new developers and is used by many who work with Android development.
  - **Kotlin**: Kotlin is a relatively new, modern, safe, and object-oriented cross-platform programming language. When Android Studio 3.0 was released in Oct 2017, Kotlin was announced as the official programming language for Android. Many popular applications such as Trello, Square, and Corda have since then shifted to Kotlin.
  - **C#**: Using the C# language developers can build native iOS and Android mobile applications.
  - **Python**: Python has emerged as one of the most popular programming languages in recent times. A dynamic and object-oriented programming language, Python is very popular in machine learning.


## Advanced

- **Name some testing scenarios for real devices, not on emulators.**
  Emulators are devices that are used to perform tasks comparable to that of real Android devices, and are used to decrease the cost of testing.  
  But some scenarios can only be performed on real devices. These scenarios include:  
    - Messaging
    - Bluetooth
    - Mounting and unmounting the memory card
    - Validation of battery scenarios
    - Memory related issues
    - Validation of the performance


- **How do you troubleshoot an application that crashes frequently?**
  The following actions can help diagnose an Android application that crashes frequently:
    - **Free Memory**: As there is a limited amount of space on mobile devices, you can try by freeing up memory space for the application to function properly
    - **Compatibility Check**: It may not be a hardware problem, but more of a software issue. It is not always possible to test an application for all devices and Operating Systems. There might be a chance that the application is not compatible with your OS, so check the compatibility on the application’s Google Play Store page.
    - **Memory Management**: Some applications run perfectly on one mobile device but may crash on other devices. This is where processing power, memory management, and CPU speed come into play. Check the application memory requirements if the application crashes constantly.
    - **App Data Usage**: You can delete the application’s data, which will clear its cache memory and allow some free space on your device and might boost the app’s performance


- **Name the different data storage options available on the Android platform.**
  Android platform provides a variety of data storage options that can be used depending on the need of the user. The storage options are:
    - **SharedPreference**: Stores data in XML files
    - **SQLite**: Stores structured data in the private database
    - **Internal Storage**: Stores data in the device file system where it cannot be read by other applications
    - **External Storage**: Stores data in the file system but it can be accessed to all apps in the device
