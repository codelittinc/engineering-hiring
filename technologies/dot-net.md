# .Net/Core

1. How does the .NET framework work?
.NET framework-based applications that are written in supportive languages like C#, F#, or Visual basic are compiled to Common Intermediate Language (CIL).
Compiled code is stored in the form of an assembly file that has a .dll or .exe file extension.
When the .NET application runs, Common Language Runtime (CLR) takes the assembly file and converts the CIL into machine code with the help of the Just In Time(JIT) compiler.
Now, this machine code can execute on the specific architecture of the computer it is running on.
2. What is .NET core?
.NET Core can be said as the newer version of the .NET Framework. It is a cost-free, general-purpose, open-source application development platform provided by Microsoft. It is a cross-platform framework because it runs on various operating systems such as Windows, Linux, and macOS. This Framework can be used to develop applications like mobile, web, IoT, machine learning, game, cloud, microservices, etc.
It consists of important features like a cross-platform, sharable library, etc., that are necessary for running a basic .NET Core application. The remaining features are supplied in the form of NuGet packages, that can be added to your application according to your needs. Like this we can say, the .NET Core will boost up the performance of an application, decreases the memory footprint, and becomes easier for maintenance of an application. It follows the modular approach, so instead of the entire .NET Framework installation, your application can install or use only what is required.
3. What is Dot NET Core used for?
.NET Core is useful in the server application creations, that run on various operating systems like Windows, Mac, and Linux. Using this, developers can write libraries as well as applications in C#, F#, and VB.NET in both runtimes.
Generally, it is used for cloud applications or for modifying large enterprise applications into microservices.
.NET Core 3.0 supports cross-development between WPF, UWP, and Windows Forms.
.NET Core supports microservices, which permits cross-platform services to work with the .NET Core framework including services developed with .NET Framework, Ruby, Java, etc.
.NET Core’s features like lightweight, modularity, and flexibility make it easier to deploy .NET Core applications in containers. These containers can be deployed on any platform, Linux, cloud, and Windows.
4. What is middleware in .NET core?
Middleware is software assembled into an application pipeline for request and response handling. Each component will choose whether the request should be passed to the next component within the pipeline, also it can carry out work before and after the next component within the pipeline.
For example, we can have a middleware component for user authentication, another middleware for handling errors, and one more middleware for serving static files like JavaScript files, images, CSS files, etc.
It can be built-in into the .NET Core framework, which can be added through NuGet packages. These middleware components are built as part of the configure method’s application startup class. In the ASP.NET Core application, these Configure methods will set up a request processing pipeline. It contains a sequence of request delegates that are called one after another.
Normally, each middleware will handle the incoming requests and passes the response to the next middleware for processing. A middleware component can take the decision of not calling the next middleware in the pipeline. This process is known as short-circuiting the pipeline or terminating the request pipeline. This process is very helpful as it avoids unnecessary work. For example, if the request is made for a static file such as a CSS file, image, or JavaScript file, etc., these static files middleware can process and serve the request and thus short-circuit the remaining pipeline.
5. What is the difference between an interface and an abstract class?
6. Does C# support multiple inheritance? No
7. What is a delegate in .NET?
A delegate is a .NET object which defines a method signature and it can pass a function as a parameter.
Delegate always points to a method that matches its specific signature. Users can encapsulate the reference of a method in a delegate object.
When we pass the delegate object in a program, it will call the referenced method. To create a custom event in a class, we can make use of delegate.