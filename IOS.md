# IOS

## High level questions

- **Explain the Architecture of iOS.**  
  iOS operates in a Layered structure. iOS Architecture is comprised of four layers, each of which offers a programming framework for creating applications that operate on top of the hardware. Communication will be enhanced by the layers between the Application Layer and the Hardware Layer. A lower-level layer provides the services that all applications require, while an upper-level layer (or high-level layer) provides graphics and interface-related services.  
  - **Core OS** ( or Application) Layer*: Core OS Layer sits directly on top of the device hardware and is the bottom layer of the iPhone OS stack. In addition to basic operating system services, such as memory management, handling of file systems, and threads, this layer provides low-level networking, access to external accessories, etc.
  - **Service Layer**: Its purpose is to design the services that upper layers or users demand. Among its other essential features are block objects, Grand Central Dispatch, in-app purchases, and iCloud storage. The service layer has been strengthened by the addition of ARC Automatic Reference Counting.
  - **Media Layer**: It handles media like video, audio, graphics, etc. The media layer will allow us to use all graphics, video, and audio technology of the system.
  - **Cocoa Touch Layer**: It is also known as the application layer. This is the place where frameworks are created when applications are built. In addition, it functions as the interface for iOS users to work with the operating system. This includes touch and motion capabilities.

- **What are different types of iOS Application States?**
  - **Not running**: In the Not Running state, an application has either not been launched or has been closed/shut down by the system.
  - **Inactive**: A brief state of inactivity occurs while the app is leaving or entering its active state. Despite running in the foreground, it isn't yet ready to accept user input or events. This means that the application remains inactive at this time.
  - **Active**: The Active state indicates that the app is running in the foreground and receiving events. This is usually the normal mode for foreground apps and the User Interface is accessible.
  - **Background**: During this state, the application's user interface is hidden, but it continues to run in the background of the iOS system. Applications usually pass through this state prior to being suspended.
  - **Suspended**: In this case, the application is in the background but is not running code. However, it stays in my memory. Under low memory conditions, the system can delete apps in the suspended state without warning.


- **Which programming languages are used for iOS development?**
  - HTML5
  - .NET
  - C
  - C++
  - Swift
  - Javascript
  - Objective-C.



- **What is deep linking in iOS?**  
Deep links are links that send users directly to an app directly instead of a website or store using URI (Uniform resource locator) or universal links. The URL scheme is a well-known method of having deep links, but Universal Links are Apple's new approach to connecting your web page and your app under the same link. Deep linking involves not only creating a clickable link that opens up your app, but also a smart one that navigates to the resource you desire. Users are directed straight to in-app locations using these links, which saves them the time and effort of finding those pages themselves thus improving their user experience tremendously. 


- **What are the different ways to achieve concurrency in iOS?**  
  Concurrency allows iOS devices to handle background tasks (such as downloading or processing data) while maintaining a responsive user interface. In iOS, you can manage concurrent tasks using Grand Central Dispatch (or GCD), and Operations (formally known as NSOperation). In order to achieve concurrency, iOS provides three ways as follows: 
  - **Dispatch queues**: They are used to manage tasks in first-in-first-out (FIFO) order and execute tasks sequentially or concurrently. This is an easy way to handle asynchronous (not occurring at the same time) and concurrent tasks in your application.
  - **Threads**: An independent sequence of instructions can be executed separately from other code within a program. Through threads, one can execute multiple code paths simultaneously in a single application. Having a thread is especially useful when you need to perform a lengthy task without affecting the execution of the rest of the program.
  - **Operation Queues**: Operation queue objects are invoked in accordance with their priority and readiness. Essentially, operation queues are high-level abstractions of queueing models, built on top of GCD (Grand Central Dispatch). It is possible, therefore, to execute tasks concurrently, just like GCD, but in an object-oriented manner.

- **How can you implement storage and persistence in iOS?**
  - Data structures such as arrays, dictionaries, sets, and other data structures are perfect for storing data intermediately.
  - NSUserDefaults and Keychains are both simple key-value stores. NSUserDefaults is insecure, whereas Keychains is secure.
  - A file or disk storage is a way to store data (serialized or not) to or from a disk using NSFileManager.
  - Relational databases, such as SQLite, are good for implementing complex querying mechanisms.



## Objective-C and Swift

- **Does Objective-C supports dynamic and static typing?**
  Yes
  
- **Explain the @dynamic and @synthesize commands in Objective-C.**
  - **@synthesize**: This command generates getter and setter methods within the property and works in conjunction with the @dynamic command. By default, @synthesize creates a variable with the same name as the target of set/get
  - **@dynamic**: This tells the compiler that the getter and setter methods are not implemented within the class itself, but elsewhere (like the superclass or that they will be available at runtime).
  
- **What are the differences between functions and methods in Swift?**
  - **Functions** are self-contained chunks of code that perform a specific task. You give a function a name that identifies what it does, and this name is used to “call” the function to perform its task when needed. With functions, there is no self.
  - **Methods** are functions that are associated with a particular type. Classes, structures, and enumerations can all define instance methods, which encapsulate specific tasks and functionality for working with an instance of a given type. The method can access self.

- **Is Swift better and Objective-C?**  
  The answer to this should consider:
    - Readability: Swift provides a better readability of the code
    - Multiplatform support: Swift is fully compatible with iOS, macOS, tvOS, watchOS, Linux, and many other platforms. This means you are able to develop software that is compatible with all operating systems.
    - Compatible with Objective C: Swift has full compatibility with Objective-C. Swift enables programmers to import frameworks from Objective-C using the Swift syntax. Programmers can utilize Objective-C libraries and classes inside Swift code.

- **What is a lazy property in iOS?**  
  Lazy properties are properties whose initial value isn't computed until the first time they are used. Including the lazy modifier/keyword before the declaration of a stored property indicates it is lazy. This lets you delay the initialization of stored properties. This could be a great way to streamline your code and reduce unnecessary work. When a code is expensive and unlikely to be called consistently, a lazy variable can be a great solution. 

- **Explain the function of the completion handler.**  
  Completion handlers are basically just functions passed as parameters to other functions. They are used to dealing with the response of asynchronous tasks since we do not know when they will end. Completion handlers inform an application when an operation, such as an API call, has been completed. The program is informed that the next step needs to be executed.  

- **When would you use Categories over Inheritance and vice versa?**  
  - If you are adding functions, but not data, use a category. An example of this is adding functions to NSMutableData which allow you to remove X bytes from a section of the data, or remove all BUT X bytes from the data. It doesn't make sense to create an entire sub-class simply to add these two functions, nor does it makes sense to write functions that aren't attached to a class (a plain C function). This allows you to attach the functionality to the class without creating a new, uneeded relationship, and doesn't change any part of existing functionality.
  - If you need to add/change data and add functionality to manipulate that data, or change functionality to represent a sub-type of object in your controller model, then you sub-class. For example, NSMutableData is a sub-class because it still uses NSData accessors, however, it changes the data representation internally so it can also manipulate the data. In this case a sub-class makes sense because it is no longer NSData, it is a /mutable/ NSData object (new keyword added to describe the object).

## Questions about publishing the app to the Apple Store

- **What is difference between App ID and Bundle ID?**   
  - Bundle ID: They are the unique identifiers of applications in Apple's ecosystem. In other words, no two applications can have the same identifier. The bundling ID is used for both OS X and iOS apps and can be used to recognize app updates. 
    Example:
      If our organization’s domain is scaler.com and we create an app named Edge, you could assign the string com.scaler.edge as our app’s bundle ID.
  - App ID: This string uniquely identifies one or more apps from the same development team. There are two components to the string, the Team ID and the Bundle ID, separated by a period (.). Apple supplies a Team ID to identify a specific development team, whereas developers supply Bundle IDs to identify a single app or a collection of apps.  
    Example:
      ABCDE12345.com.scaler.edge
      In the above example, ABCDE12345 is the Team ID and com.scaler.edge is the Bundle ID.
      
- **Explain code signing for iOS apps.**
Signing an application allows the system to identify who signed the application and to verify that the application has not been modi ed since it was signed. Signing is a requirement for submitting to the App Store (both for iOS and Mac apps). OS X and iOS verify the signature of applications downloaded from the App Store to ensure that they they do not run applications with invalid signatures. This lets users trust that the application was signed by an Apple source and hasn’t been modifed since it was signed.


