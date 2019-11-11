# iOS-interview

## <a name='contents'>Table of Contents</a>
* [Preparation](#preparation)
* [Phone Screen](#phone-screen)
* [ON SITE](#on-site)
-----------
* [iOS](#iOS)
* [Patterns](#Patterns)
-----------

# Preparation
[[⬆]](#contents)
-----------

## Portfolio
<details><summary>Portfolio</summary>
1. http://www.inheritx.com/
2. http://100grams.nl/
3. http://ios-developer.fr/
4. scalsys.com
5. http://www.aichtechnologies.com/portfolio.php
6. https://ekatsuta.github.io/index.html
7. [CV](https://www.careercup.com/resume)
</details>

## iOS(swift):
### Theory - [swift-book](https://docs.swift.org/swift-book/) 
### Practical(swift knowledge) - [swift](https://repl.it/@dmyma/Swift-knowledge) 
### Practical(iOS knowledge) - [raywenderlich.com/](https://www.raywenderlich.com/)

## Data Structures and Algorythms - [leetcode](leetcode.com)
### Alg:
- [Leetcode](https://leetcode.com/)
- [G4G](https://www.geeksforgeeks.org)
- [CTCI](https://www.amazon.com/Cracking-Coding-Interview-Programming-Questions/dp/0984782850)
- [EPI](https://www.amazon.com/Elements-Programming-Interviews-Python-Insiders/dp/1537713949)
- [CF](http://codeforces.com)
- [CC](codechef.com)

### DS:
- [Alg 4th](https://www.amazon.com/gp/product/032157351X)
- [Alg Design](https://www.amazon.com/gp/product/1849967202)
- [Intro](https://www.amazon.com/Introduction-Algorithms-3rd-MIT-Press/dp)
- [class SU](https://www.coursera.org/specializations/algorithms)
- [Google](https://www.udacity.com/course/data-structures-and-algorithms-in-python--ud513)
- [mycodeschool](https://www.youtube.com/watch?v=92S4zgXN17o&list=PL2_aWCzGMAwI3W_JlcBbtYTwiQSsOTa6P)
- [MIT](https://www.youtube.com/watch?v=HtSuA80QTyo&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb)

## System Design / Object Oriented Design - [premier](https://github.com/donnemartin/system-design-primer)
### System Design
- [101](https://engineering.videoblocks.com/web-architecture-101-a3224e126947)
- [pramp](https://github.com/donnemartin/system-design-primer)
- [GSDI](https://www.educative.io/collection/5668639101419520/5649050225344512)
- [youtube](https://www.youtube.com/watch?v=UzLMhqg3_Wc)
- [youtube2](https://www.youtube.com/watch?v=jItLuOTsCX4)
- [HT](https://www.hiredintech.com/courses/system-design)
- [HS](http://highscalability.com/)

### Object Oriented Design:
- [GOOPI](https://www.educative.io/courses/grokking-the-object-oriented-design-interview)
- [PDG4](https://www.educative.io/courses/software-design-patterns-best-practices/xVovQB3Rknq)
- [Patterns of Design](https://github.com/ochococo/Design-Patterns-In-Swift)
- [Patterns](https://sourcemaking.com/design_patterns)

## Behavioral - [Amazon 14 principals](https://www.youtube.com/watch?v=RzlUQCy84rQ)

# Phone Screen
[[⬆]](#contents)
-----------

## Theory
1. class vs struct
2. frame vs bounds + scroll view
3. GCD vs NSOperationQueue(async, sync, gcd, queues, operations, threades)
4. MVVM vs MVC vs MVP vs Viper
5. ARC + ObjC
6. App LifeCycle, View LifeCycle
7. delegate vs notification center vs callback
8. Gesture recogniser
9. URL session request
10. init
11. How protocols interact with generics
12. Generics
12. Protocols: Hashable, HashFunctions, Codable
14. objC NULL, inter
15. Networking
16. Testing
17. filter, map, reduce, flatMAP, modulo
18. 3D party libraries
19. debugging
20. autolayout/sizeclasses
21. Optional biding 
22. Initializers

## Practical
1. Create a button and drag it around in code
2. Parse json
3. Networking get request and then post
4. Authentication
5. Navigation
6. Pass objects around
7. If you had a home project you can add some features or discuss your solution

## Algorithms
Usually there are two questions and each can have a follow up.
1. [esay](https://leetcode.com/problems/valid-parentheses/)
2. [medium](https://leetcode.com/problems/evaluate-reverse-polish-notation/)


# On site
[[⬆]](#contents)
-----------

## iOS
1. Write Generic Stack implementation
2. Write json parser
3. Create a quez app
4. If you had a home project you can add some features or discuss your solution

## System Design
1. Design a Callendar application
2. Design a Chat application
3. Design Twitter
4. Scalability
5. Multithreading

## DSA
1. HashMap
2. Binary Search
3. Merge Sort
4. KMP and Rabin-Karp
5. BFS and DFS
6. DP
7. Strings
8. Graphs: Trees, BT, BST, RB Tree, AB Tree, Segmented Tree, AVL
9. Sliding Window
10. 2 Pointers or Iterators
11. Fast and Slow Pointers or Iterators: Floyd's Tortoise and Hare
12. Merge Intervals
13. In-place reversal of linked list
14. Heaps
15. Topological sort: MST, Prim(min), Kruskal(connected)
16. Union Find
17. Shortest Path: Dijkstra, Bellman Ford(n-1), Floyd Warshall(all), Johnson, A* star 
18. Kaddan 
19. Huffman coding

## Behavioral
1. Tell me a project you have worked that you found out it could be much bigger after you started working on this
2. Tell me a project where you had to work with tight deadlines.
3. Tell me a project where you had to analyze the initial solution and then found a differnet solution for the problem.
4. Sometimes there questions to find out if you are a leader or a manager.



## iOS 
[[⬆]](#contents)
-----------
<details><summary>What is the diference between struct and class?</summary>
An  enum  is an object type whose instances represent  distinct  predefined  alternative values. Think of it as a list of known possibilities. An enum is the Swift way to express a set of constants that are alternatives to one another. An enum declaration includes case statements. Each case is the name of one of the alternatives. An instance of an enum will represent exactly one alternative — one case.

Methods A  method  is a function — one that happens to be declared at the top level of an object type declaration. This means that everything said about functions in  Chapter 2 applies. By default, a metho

Properties A  property  is a variable — one that happens to be declared at the top level of an object type declaration. This means that everything said about variables in  Chapter 3 applies. A property has a fixed type; it can be declared with  var  or  let; it can be stored or computed; it can have setter observers. An instance property can also be declared  lazy.

Structs A  struct  is the Swift object type  par excellence. An enum, with its fixed set of cases, is a reduced, specialized kind of object. A class, at the other extreme, will often turn out to be overkill; it has some features that a struct lacks, but if you don’t need those features, a struct may be preferable.

Classes A  class  is similar to a struct, with the following key differences: Reference type Classes are reference types. This means, among other things, that a class instance has two remarkable features that are not true of struct instances or enum instances: Mutability A class instance is mutable in place. Even if your reference to an instance of a class is a constant (let), you can change the value of an instance property through that reference. An instance method of a class never has to be marked  mutating  (and cannot be). Multiple references When a given instance of a class is assigned to multiple variables or passed as argument to a function, you get multiple references to  one and the same object. Inheritance A class can have a superclass. A class that has a superclass is a  subclass  of that superclass. Class types can thus form a hierarchical tree. In Objective-C, classes are the only object type. Some built-in Swift struct types are magically bridged to Objective-C class types, but your custom struct types don’t have that magic. Thus, when programming iOS with Swift, a primary reason for declaring a class, rather than a struct, is as a form of interchange with Objective-C and Cocoa.

Value Types and Reference Types A major difference between enums and structs, on the one hand, and classes, on the other, is that enums and structs are  value types, whereas classes are  reference types. A value type is  not mutable in place, even though it seems to be. For example, consider a struct. A struct is a value type:
</details>

<details><summary>App Delegate Methods</summary>
-UIApplicationDidFinishLaunching
-UIApplicationWillResignActive
-UIApplicationDidBecomeActive
-UIApplicationWillEnterForeground
-UIApplicationDidEnterBackground
-UIApplicationwillterminate
	</details>
<details><summary>App States</summary>
### States

Apps developed for early iOS versions (before iOS 4.0) supported three states: non-running, inactive, and active. An application delegate for pre-iOS 4.0 apps received two important method calls: applicationDidFinishLaunching and applicationWillTerminate. When an app received an applicationDidFinishLaunching message, it was an opportunity for information to be retrieved from the previous launch to restore the app to its last used state. The status, applicationWillTerminate, was used to notify the app when the app was preparing to shut down. This gave the developer an opportunity to save any unsaved data or specific state information.

Currently, there are five possible application states that would be cause for the app to prepare for a transition - such as a shutdown or moving to the background. In certain cases, an app might need to continue processing in the background. However, there is certainly no reason for the app to process any graphics, animations, or display-specific routines. The five states of an iOS app - as listed in the iOS App Programming Guide - include the following:

- Non-running - The app is not running.
- Inactive - The app is running in the foreground, but not receiving events. An iOS app can be placed into an inactive state, for example, when a call or SMS message is received.
- Active - The app is running in the foreground, and receiving events.
- Background - The app is running in the background, and executing code.
- Suspended - The app is in the background, but no code is being executed.
- The seven most important application delegate methods

The operating system calls specific methods within the application delegate to facilitate transitioning to and from various states. The seven most important application delegate methods a developer should handle are:

### application:willFinishLaunchingWithOptions
Method called when the launch process is initiated. This is the first opportunity to execute any code within the app.

### application:didFinishLaunchingWithOptions
Method called when the launch process is nearly complete. Since this method is called is before any of the app's windows are displayed, it is the last opportunity to prepare the interface and make any final adjustments.

### applicationDidBecomeActive
Once the application has become active, the application delegate will receive a callback notification message via the method applicationDidBecomeActive.

This method is also called each time the app returns to an active state from a previous switch to inactive from a resulting phone call or SMS.

### applicationWillResignActive
There are several conditions that will spawn the applicationWillResignActive method. Each time a temporary event, such as a phone call, happens this method gets called. It is also important to note that "quitting" an iOS app does not terminate the processes, but rather moves the app to the background.

### applicationDidEnterBackground
This method is called when an iOS app is running, but no longer in the foreground. In other words, the user interface is not currently being displayed. According to Apple's UIApplicationDelegate Protocol Reference, the app has approximately five seconds to perform tasks and return. If the method does not return within five seconds, the application is terminated.

### applicationWillEnterForeground
This method is called as an app is preparing to move from the background to the foreground. The app, however, is not moved into an active state without the applicationDidBecomeActive method being called. This method gives a developer the opportunity to re-establish the settings of the previous running state before the app becomes active.

### applicationWillTerminate
This method notifies your application delegate when a termination event has been triggered. Hitting the home button no longer quits the application. Force quitting the iOS app, or shutting down the device triggers the applicationWillTerminate method. This is the opportunity to save the application configuration, settings, and user preferences.

### Application state changes

Every iOS app is always in one of the five app states. The operating system manages the app state, but the app itself is responsible for managing important tasks to ensure smooth transitions between the states. Developers are required to respond appropriately to app state transitions.

With multitasking capability, the latest iOS version manages the resources available to every app. It is important to note, however, that the operating system limits what an app can do in the background. If an app needs to continue running in the background (with limited functionality), you must request permission.

### Launching the app

The moment a user taps the app icon, the app begins to change state. The app delegate receives an application:willFinishLaunchingWithOptions method call, and the app state changes from non-running to inactive. Once in the inactive state, the app delegate will receive an application:didFinishLaunchingWithOptions method call, giving the app an opportunity to make final adjustments before the interface is displayed. If the app has not been designed to launch in the background, the operating system will activate the app, set the app state to active, and send the applicationDidBecomeActive method call to the app delegate.

### Interruptions

On occasion, the iOS app will need to respond to interruptions. An alert-based interruption - such as a phone call - causes the app to move into an inactive state. The app delegate will receive an applicationWillResignActive method call, allowing the app an opportunity to prepare for a temporary inactive state. If the user chooses to ignore the interruption, or the interrupting process has terminated, the app will move back into the active state. While making the transition from inactive to active, the app delegate will receive an applicationDidBecomeActive method call.

### Switching to the background

The iOS devices make it simple to quickly switch from app to app; when a user switches to a different app, the current app moves to the background. The app can be in one of two states: background or suspended. In either case, and before switching to the background, the app delegate receives an applicationWillResignActive method call, followed by an applicationDidEnterBackground message. If in a suspended state, the app sleeps. A background state - meaning that the app is allowed to continue executing code - requires the app to monitor and handle events. Developers need to be aware that the operating system may terminate the app at any time.#
</details>
<details><summary>UIViewController lifecycle</summary>
viewDidLoad - update UI, outlets are set, bounds not set yet(no geometry)
viewWillApear - changing over display, geometry set, optimise performance,
viewWillLAyoutSubviews - called when frames changed
viewDidlayoutSubviews
viewDidApear - 
viewWillDisapear - remember whats going on and clean up, no time consuming
viewDidDisapear
</details>
<img src="Lifecycle.png" width="301" height="400"> 
<img src="PushNotifications.png" width="301" height="400">
<details><summary>Memory Management</summary>
- Core Data
- SQL
- Realm
</details>

<details><summary>Advanced Threading</summary>
	[mutex](http://www.lukeparham.com/blog/2018/6/3/comparing-synchronization-strategies)
	[fairness](https://www.mikeash.com/pyblog/friday-qa-2017-10-27-locks-thread-safety-and-swift-2017-edition.html)
	- thread vs queue[link](https://stackoverflow.com/questions/23166246/what-is-the-difference-between-thread-and-queue-in-ios-development)
	- load vs initialize[link](https://www.mikeash.com/pyblog/friday-qa-2009-05-22-objective-c-class-loading-and-initialization.html)
	</details>
<details><summary>NSThread vs NSOperation</summary>
NSThread:

1. iOS developers have to write code for the work/process he want to perform along with for the creation and management of the threads themselves.
2. iOS developers have to be careful about a plan of action for using threads.
3. iOS developer have to manage posiable problems like reuseability of thread, lockings etc. by them self.
4. Thread will consume more memory too.

NSOperation:

1. The NSOperation class is an abstract class which encapsulates the code and data associated with a single task.
2. Developer needs to use subclass or one of the system-defined subclasses of NSOperation to perform the task.
3. Add operations into NSOperationQueue to execute them.
4. The NSOperationQueue creates a new thread for each operation and runs them in the order they are added.
5. Operation queues handle all of the thread management, ensuring that operations are executed as quickly and efficiently as possible.
6. An operation queue executes operations either directly by running them on secondary threads or indirectly using GCD (Grand Central Dispatch).
7. It takes care of all of the memory management and greatly simplifies the process.
8. If you don’t want to use an operation queue, you can also execute an operation by calling its start method. It may make your code too complex.
</details> 

  
  <details><summary> Explain NSURLSession?</summary>
  The NSURLSession class and related classes provide an API for downloading content via HTTP. This API provides a rich set of delegate methods for supporting authentication and gives your app the ability to perform background downloads when your app is not running or, in iOS, while your app is suspended.

To use the NSURLSession API, your app creates a series of sessions, each of which coordinates a group of related data transfer tasks. For example, if you are writing a web browser, your app might create one session per tab or window. Within each session, your app adds a series of tasks, each of which represents a request for a specific URL (and for any follow-on URLs if the original URL returned an HTTP redirect).

Like most networking APIs, the NSURLSession API is highly asynchronous. If you use the default, system-provided delegate, you must provide a completion handler block that returns data to your app when a transfer finishes successfully or with an error. Alternatively, if you provide your own custom delegate objects, the task objects call those delegates' methods with data as it is received from the server (or, for file downloads, when the transfer is complete).

Note: Completion callbacks are primarily intended as an alternative to using a custom delegate. If you create a task using a method that takes a completion callback, the delegate methods for response and data delivery are not called.
The NSURLSession API provides status and progress properties, in addition to delivering this information to delegates. It supports canceling, restarting (resuming), and suspending tasks, and it provides the ability to resume suspended, canceled, or failed downloads where they left off.</details>
  <details> 
  <summary> Explain types of NSURLSession?</summary>
  The NSURLSession API supports three types of sessions, as determined by the type of configuration object used to create the session:

- Default sessions : behave similarly to other Foundation methods for downloading URLs. They use a persistent disk-based cache and store credentials in the user's keychain.

- Ephemeral sessions : do not store any data to disk; all caches, credential stores, and so on are kept in RAM and tied to the session. Thus, when your app invalidates the session, they are purged automatically.

- Background sessions : are similar to default sessions, except that a separate process handles all data transfers. Background sessions have some additional limitations.
</details>
  
  <details> 
  <summary> Explain life cycle of URL Session?</summary>
  You can use the NSURLSession API in two ways: with a system-provided delegate or with your own delegate. In general, you must use your own delegate if your app does any of the following:

- Uses background sessions to download or upload content while your app is not running.
- Performs custom authentication.
- Performs custom SSL certificate verification.
- Decides whether a transfer should be downloaded to disk or displayed based on the MIME type returned by the server or other similar criteria.
- Uploads data from a body stream (as opposed to an NSData object).
- Limits caching programmatically.
- Limits HTTP redirects programmatically.

If your app does not need to do any of these things, your app can use the system-provided delegates. Depending on which technique you choose, you should read one of the following sections:

- Life Cycle of a URL Session with System-Provided Delegates : provides a lightweight view of how your code creates and uses a URL session. You should read this section even if you intend to write your own delegate, because it gives you a complete picture of what your code must do to configure the object and use it.

- Life Cycle of a URL Session with Custom Delegates : provides a complete view of every step in the operation of a URL session. You should refer to this section to help you understand how the session interacts with its delegate. In particular, this explains when each of the delegate methods is called.


</details>


<details><summary>async vs sync</summary>
[GCD vs Q](http://www.knowstack.com/swift-3-1-concurrency-operation-queue-grand-central-dispatch/)

</details>
<details> 
  <summary>core data and different threads</summary>

Basic rules are:

Use one NSPersistentStoreCoordinator per program not per thread.
Create one NSManagedObjectContext per thread.
Never pass an NSManagedObject on a thread to the other thread.
Instead, get the object IDs via -objectID and pass it to the other thread.
More rules:

Make sure you save the object into the store before getting the object ID. Until saved, they're temporary, and you can't access them from another thread.
And beware of the merge policies if you make changes to the managed objects from more than one thread.
NSManagedObjectContext's -mergeChangesFromContextDidSaveNotification: is helpful.
Documentation
https://cocoacasts.com/core-data-and-concurrency/
https://www.raywenderlich.com/145877/core-data-tutorial-multiple-managed-object-contexts-2
</details>
<details> 
  <summary> What steps should be accomplish in order to save/fetch an object?  </summary>
Step 1  —  Describes which entity we are working with. LEts say Person.
Step 2  —  Create the our Class(PErson) NSManagedObject. The NSManagedObject will be inserted into our managed object context later when saving.
Step 3  —  Now that we have specified our entity and created a new class(person), we need to save the person’s name. In this case, we use key value coding to set the value for our key, which is specified as “name”.
Step 4  —  At this point, it’s time to save our managedObjectContext, which persists the data to the store. If an error should occur, we catch it at this point.
- Fetch
Step 1  —  Create a fetch request. A fetch request is what we use to fetch data from our Core Data store. A fetch request can be customizable to include only the results or attributes that you need. In our case, we want to fetch all objects from the Person entity.
Step 2  —  We now try to fetch data from our Core Data store and store it in our managed object context, whose job it is to create a scratchpad of sorts when dealing with managed objects.
Step 3  —  We have a simple for loop that loops through each result in our fetched items array. At this point, we print out the name of each saved object into the console.
	
https://www.codementor.io/codementorteam/core-data-tutorial-saving-and-fetching-pdphdmh50
https://developer.apple.com/library/content/documentation/Cocoa/Conceptual/CoreData/CreatingObjects.html


Application-(Managed Object Contex(Manage Object))- Persistance storage Coordinator(PS Model) - PS
</details>
<details><summary>point(inside:with:) vs hitTest(_:with:)</summary></details>
<details><summary>NSAttributedString</summary></details>

<details><summary>Swift futures</summary>
Fast and concise iteration over a range or collection
Structs that support methods, extensions, and protocols
Functional programming patterns, e.g., map and filter
Powerful error handling built-in
Advanced control flow with do, guard, defer, and repeat keywords
</details>
<details><summary>nil in Swift vs nil in Objective-C? Difference?</summary>
In defintion terms:

Swift optional variable is an enum, which can have nil as a value, where as objective variable is a pointer, where nil represents, it is pointing no where.

In Usage terms:

Both are somewhat similar in the sense,

that both variables having nil value on messaging any method returns nil

Optional chaining in Swift is similar to messaging nil in Objective-C, but in a way that works for any type, and that can be checked for success or failure.
But in Safety Checking, Swift optional is the winner

As compiler does many type checking for you already, Ex. non optional parameter can't accept optional, thus you will need to unwrap it by first checking it for nil Or when you you cast any variable, it always returns an optional, thus again a safety feature at compiler level</details>

<details> 
  <summary> What’s the difference between the frame and the bounds? </summary>
   The bounds of an UIView is the rectangle, expressed as a location (x,y) and size (width,height) relative to its own coordinate system (0,0). 
The frame of an UIView is the rectangle, expressed as a location (x,y) and size (width,height) relative to the superview it is contained within.
</details>


<details> 
  <summary> What is the use of controller object UIApplication?</summary>
Controller object UIApplication is used without subclassing to manage the application event loop.
It coordinates other high-level app behaviors. 
It works along with the app delegate object which contains app-level logic.
</details>

<details> 
  <summary> Which object is create by UIApplicationMain function at app launch time?</summary>
The app delegate object is created by UIApplicationMain function at app launch time. The app delegate object's main job is to handle state transitions within the app.
</details>

<details> 
  <summary> How is the app delegate is declared by Xcode project templates?</summary>
App delegate is declared as a subclass of UIResponder by Xcode project templates.
</details>

<details> 
  <summary> What happens if IApplication object does not handle an event?</summary>
In such case the event will be dispatched to your app delegate for processing.
</details>

<details> 
  <summary> Which app specific objects store the app's content?</summary>
Data model objects are app specific objects and store app’s content. Apps can also use document objects to manage some or all of their data model objects.
</details>

<details> 
  <summary> Are document objects required for an application? What does they offer?</summary>
Document objects are not required but are very useful in grouping data that belongs in a single file or file package.
</details>

<details> 
  <summary>  Which object manage the presentation of app's content on the screen?</summary>
View controller objects takes care of the presentation of app's content on the screen. A view controller is used to manage a single view along with the collection of subviews. It makes its views visible by installing them in the app’s window.
</details>

<details> 
  <summary> Which is the super class of all view controller objects?</summary>
UIViewController class. The functionality for loading views, presenting them, rotating them in response to device rotations, and several other standard system behaviors are provided by UIViewController class.
</details>

<details> 
  <summary> What is the purpose of UIWindow object?</summary>
The presentation of one or more views on a screen is coordinated by UIWindow object.
</details>


<details> 
  <summary>When an app is said to be in not running state? </summary>
An app is said to be in 'not running' state when: 
- it is not launched. 
- it gets terminated by the system during running.
</details>

<details> 
  <summary>Assume that your app is running in the foreground but is currently not receiving events. In which sate it would be in? </summary>
An app will be in InActive state if it is running in the foreground but is currently not receiving events. An app stays in InActive state only briefly as it transitions to a different state.
</details>

<details> 
  <summary>Give example scenarios when an application goes into InActive state? </summary>
An app can get into InActive state when the user locks the screen or the system prompts the user to respond to some event e.g. SMS message, incoming call etc.
</details>

<details> 
  <summary>When an app is said to be in active state? </summary>
An app is said to be in active state when it is running in foreground and is receiving events.
</details>

<details> 
  <summary> Name the app sate which it reaches briefly on its way to being suspended. </summary>
An app enters background state briefly on its way to being suspended.
</details>

<details> 
  <summary> Assume that an app is not in foreground but is still executing code. In which state will it be in? </summary>
Background state.
</details>

<details> 
  <summary>An app is loaded into memory but is not executing any code. In which state will it be in? </summary>
An app is said to be in suspended state when it is still in memory but is not executing any code.
</details>

<details> 
  <summary>Assume that system is running low on memory. What can system do for suspended apps? </summary>
In case system is running low on memory, the system may purge suspended apps without notice.
</details>

<details> 
  <summary>How can you respond to state transitions on your app? </summary>
On state transitions can be responded to state changes in an appropriate way by calling corresponding methods on app's delegate object.

applicationDidBecomeActive method can be used to prepare to run as the foreground app. 
applicationDidEnterBackground method can be used to execute some code when app is running in the background and may be suspended at any time. 
applicationWillEnterForeground method can be used to execute some code when your app is moving out of the background 
applicationWillTerminate method is called when your app is being terminated.
</details>

<details> 
  <summary>List down app's state transitions when it gets launched. </summary>
Before the launch of an app, it is said to be in not running state.
When an app is launched, it moves to the active or background state, after transitioning briefly through the inactive state.
</details>

<details> 
  <summary>Who calls the main function of you app during the app launch cycle? </summary>
During app launching, the system creates a main thread for the app and calls the app’s main function on that main thread. The Xcode project's default main function hands over control to the UIKit framework, which takes care of initializing the app before it is run.
</details>



<details> 
  <summary> Define view object.</summary>
Views along with controls are used to provide visual representation of the app content. View is an object that draws content in a designated rectangular area and it responds to events within that area.
</details>


<details> 
  <summary> Apart from incorporating views and controls, what else an app can incorporate?</summary>
Apart from incorporating views and controls, an app can also incorporate Core Animation layers into its view and control hierarchies.
</details>

<details> 
  <summary> What are layer objects and what do they represent?</summary>
Layer objects are data objects which represent visual content. Layer objects are used by views to render their content. Custom layer objects can also be added to the interface to implement complex animations and other types of sophisticated visual effects.
</details>

<details> 
  <summary> What are the levels of privacy in swift 3?</summary>



Swift 3 has five levels of privacy: internal The default rule is that declarations are  internal, meaning that they are globally visible to  all code in all  files  within the containing module.  That is why Swift files within the same module can see one another’s top-level contents  automatically, with no effort on your part. (That’s different from C and Objective-C, where files can’t see each other at all unless you explicitly show them to one another through include  or  import  statements.) fileprivate  (narrower than  internal) A thing declared  fileprivate  is visible  only within its containing  file.  For example, two object types declared in the same file can see one another’s members declared  fileprivate, but code in other files cannot see those members. private  (even narrower than  fileprivate) A thing declared  private  is visible  only within its containing curly braces. In effect, the visibility of an object type’s member declared  private  is limited to code within this class declaration. (A  private  declaration at the top level of a file is equivalent to  fileprivate.) public  (wider than  internal) A thing declared  public  is visible  even outside its containing module.  Another module must first import this module before it can see anything at all. But once another module  has  imported this module, it still won’t be able to see anything in this module that hasn’t been explicitly declared public. If you don’t write any modules, you might never need to declare anything public. If you do write a module, you  must  declare  something  public, or your module is useless. open  (even wider than  public) If a class is declared  open, code in another module can subclass it; it can’t do that if the class is declared merely  public. If an open class member is declared  open, code in another module that subclasses this class can override
</details>

<details><summary>When init method needed?</summary>
init method are not so common because properties can have their defaults set using =
or properties can be optionals
you can use lazy
So you only need init when a value can’t be set in any of these ways</details>


1. <details><summary>let vs var</summary></details>
2. <details><summary>Collection in Swift</summary></details>
3. <details><summary>raw Value vs associated</summary></details>
4. <details><summary>If the app crashes what would you do?</summary></details>
5. <details><summary>Singleton</summary></details>
6. <details><summary>Ex. states of the app</summary></details>
7. <details><summary>Swift vs ObjC</summary></details>
8. <details><summary>Codable</summary></details>
9. <details><summary>typles</summary></details>
10. <details><summary>map, filter, reduce</summary>
```swift
	extension Array {
    func map<T>(_ transform: (Element) -> T) -> [T] {
        var result: [T] = []
        for element in self {
            result.append(transform(element))
        }
        return result
    }
}
```


```swift
extension Array {
    func filter(_ includeElement: (Element) -> Bool) -> [Element] {
        var result: [Element] = []
        for element in self where includeElement(element) {
            result.append(element)
        }
        return result
    }
}
```


```swift
extension Array {
    func reduce<T>(_ initialResult: T, combiner: (T, Element) -> T) -> T {
        var result: T = initialResult
        for element in self {
            result = combiner(result, element)
        }
        return result
    }
}
```

</details>
11. <details><summary>guard</summary></details>
12. <details><summary>class vs struct</summary></details>
13. <details><summary>error handling</summary>do, try, catch</details>
14. <details><summary>closure vs delegate vs notification</summary>
	* closure only on method
	* delegate foe an object
	* notification many to many
</details>

15. <details><summary>Inheritance vs Composition</summary></details>
16. <details><summary>Bridge header and @objC</summary></details>
17. <details><summary>Documentation</summary></details>


<details><summary>More</summary>
1. What is Optional in Swift and nil in Swift and Objective-C?
2. What are properties and instance variables in Objective-C and Swift?
3. What is a protocol (both Obj-C and Swift)? When and how is it used?
4. What is a category/extension? When is it used?
5. What are closures/blocks and how are they used?
6. What is MVC?
7. What are Singletons? What are they used for?
8. What is Delegate pattern in iOS?
9. What is KVO (Key-Value Observation)?
10. What are CGRect Frames? When and where would you use them?
11. What is AutoLayout? When and where would you use it?
12. What are compression resistance and content hugging priorities for?
13. How does AutoLayout work with multi-threading?
14. What are the advantages and disadvantages of creating AutoLayouts in code versus using storyboards?
15. How do you work with storyboards in a large team?
16. How do you mix AutoLayout with Frames?
17. What options do you have with animation on iOS?
18. How do you do animation with Frames and AutoLayout?
19. How do you work with UITableView?
20. How do you optimize table views performance for smooth, fast scrolling?
21. How do you work with UICollectionView?
22. How do you work with UIScrollView?
23. What is UIStackView? When would you use it and why?
24. What design patterns are commonly used in iOS apps?
25. What are SOLID principles? Can you give an example of each in iOS/Swift?
26. How do you manage dependencies in iOS applications?
27. What is Functional Programming and Functional Reactive Programming?
28. MRC vs ARC? What is it? How does it work? What is the main principle?
29. Autorelease pool, when? Next drain 
30. Objective-C properties(strong, weak, copy(which: nscopy protocol to support the , assign ) copy vs assigned
31. Origin of bounds equals zero(rotate the view or move inside of the super view) like scroll view, frame the same bound change
32. Problem: small button(put a view on top with Gesture recogniser, bigger button, on set of the button, responderchain(hitTest, property Animator) if the touch inside of the view or outside
33. What are the ways to animate view(animate, core animation)property animate 
34. GCD vs NSOperationQueue, dispatch queue which is concurant(, dispatch after do?, where it can be useful , dispatchgroup, dispatch barrier async (only one at a time) , dispatch queue how to synchronize ? Locks
35. what is deadlock? How to avoid deadlocks 
</details> 

## Patterns 
[[⬆]](#contents)
-----------

<img src="designpatterns1.jpg" width="301" height="400">
<img src="designpatterns2.jpg" width="301" height="400">

<details><summary>Singleton</summary> - ensures a class has only one instance and provides global point of access to it </details>
<details><summary>Factory Method</summary> - define an interface for creating an object, but let the subclass decide which class to instantiate</details>
<details><summary>ABS</summary> - provides an interface for creating families of related or depended objects without specifying heir concrete classes</details>
<details><summary>Builder</summary> - separates the construction of a complex object from its representation so the same construction process can create different representations</details>
<details><summary>Prototype</summary> - specify the kinds of objects to create using a prototypical instance, and creating new object by copying this prototype</details>

<details><summary>Adapter</summary>  - provides a link between two otherwise incompatible types by wrapping the "adaptee" with a class that supports the interface required by the client.</details>
<details><summary>Bridge</summary>  - separates the abstract elements of a class from the implementation details, providing the means to replace the implementation details without modifying the abstraction.</details>
<details><summary>Facade</summary>  - define a simplified interface to a more complex system(API)</details>
<details><summary>Flyweight</summary>  - minimizes memory usage or computational expenses by sharing as much as possible with other similar objects.</details>
<details><summary>Proxy</summary>  - provide a surrogate or placeholder object, which reference an underlying object.( virtual - load objects on demand, protection - restricting access)</details>
<details><summary>Template Method</summary>  - The Template Pattern is used when two or more implementations of an algorithm exist. The template is defined and then built upon with further variations. Use this method when most (or all) subclasses need to implement the same behavior. Traditionally, this would be accomplished with abstract classes and protected methods (as in Java). However in Swift, because abstract classes don't exist (yet - maybe someday), we need to accomplish the behavior using interface delegation.(N:  Define the skeleton of an  algorithm in an operation, deferring some steps to subclasses. Template Method lets subclasses redefine certain steps of an algorithm without changing  the algorithm's structure.  )</details>
<details><summary>Observer</summary>  - allows an object to publish changes to its state. Other objects subscribe to be immediately notified of any changes.</details>
<details><summary>Decorator</summary>  - extends or alters the functionality of objects at run- time by wrapping them in an object of a decorator class. This provides a flexible alternative to using inheritance to modify behaviour.(coffee)</details>

<details><summary>Chain of Responsibility</summary> -  processes varied requests, each of which may be dealt with by a different handler.</details>
<details><summary>Strategy</summary> - creates an interchangeable family of algorithms from which the required process is chosen at run-time.</details>
<details><summary>State</summary></details>
<details><summary>Memento</summary> (Originator, caretaker) captures the current state of an object and store it in such a manner that it can be restored at a later time without breaking the rules of encapsulation.</details>


<details><summary>Visitor</summary> - separates a relatively complex set of structured data classes from the functionality that may be performed upon the data that they hold.</details>


<details><summary>Command</summary> - expresses a request, including the call to be made and all of its required parameters, in a command object. The command may then be executed immediately or held for later use.</details>
<details><summary>Composite</summary> - creates hierarchical, recursive tree structures of related objects where any element of the structure may be accessed and utilised in a standard manner.</details>

<details><summary>Mediator</summary> reduces coupling between classes that communicate with each other. Instead of classes communicating directly, and thus requiring knowledge of their implementation, the classes send messages via a mediator object.</details>
<details><summary>Interpreter</summary></details>
<details><summary>Iterator</summary></details>
<details> <summary>What is OOP?</summary>
Inheritance - allowas a class to be definde as a modified or more specialized version of another class
Polymorphism - the capability to provide multiple implementations of an action and to select the correct implementation based on the surrounding context.override</details>
<details> <summary>What is POP?</summary></details>

interface, abstract class class/protocol
<details> <summary>What are the pros and cons of inheritance?</summary></details>
<details> <summary>What is polymorphism?</summary></details>
<details> <summary>What is tight coupling?</summary></details>
<details> <summary>What are design patterns and how they are good?</summary></details>
<details> <summary>Tell me some important design patterns used in iOS?</summary></details>
<details> <summary>What is singleton?</summary></details>
<details> <summary>What challenges you have encounter implementing MVC?</summary></details>
<details> <summary>What is MVVM and why you will use it?</summary></details>
<details> <summary>What is dependency injection, how it is good?</summary></details>

<details> <summary>Decorator vs Inheritance</summary></details>
<details> <summary>App Architecture</summary>
1. MVC
2. Viper
3. MVP
4. MVVC
5. MVVM-C
6. MVVM-A

http://gexiaoguo.github.io/MVC,-MVP-and-MVVM/
</details>


