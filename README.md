# iOS-interview

## <a name='contents'>Table of Contents</a>
* [Preparation](#preparation)
* [Phone Screen](#phone-screen)
* [ON SITE](#on-site)
-----------
* [Cocoa touch](#cocoa-touch)
-----------

# Preparation
[[⬆]](#preparation)
-----------
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

### Behavioral - [Amazon 14 principals](https://www.youtube.com/watch?v=RzlUQCy84rQ)

# Phone Screen
[[⬆]](#phone-screen)
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



## Cocoa touch 
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
<details><summary>What is Optional in Swift and nil in Swift and Objective-C?</summary></details>
<details><summary>What are properties and instance variables in Objective-C and Swift?</summary></details>
<details><summary>What is a protocol (both Obj-C and Swift)? When and how is it used?</summary></details>
<details><summary>What is a category/extension? When is it used?</summary></details>
<details><summary>What are closures/blocks and how are they used?</summary></details>
<details><summary>What is MVC?</summary></details>
<details><summary>What are Singletons? What are they used for?</summary></details>
<details><summary>What is Delegate pattern in iOS?</summary></details>
<details><summary>What is KVO (Key-Value Observation)?</summary></details>
<details><summary>What does iOS application lifecycle consist of?</summary></details>
<details><summary>What is View Controller? What is its lifecycle?</summary></details>


<details><summary>What are CGRect Frames? When and where would you use them?</summary></details>
<details><summary>What is AutoLayout? When and where would you use it?</summary></details>
<details><summary>What are compression resistance and content hugging priorities for?</summary></details>
<details><summary>How does AutoLayout work with multi-threading?</summary></details>
<details><summary>What are the advantages and disadvantages of creating AutoLayouts in code versus using storyboards?</summary></details>
<details><summary>How do you work with storyboards in a large team?</summary></details>
<details><summary>How do you mix AutoLayout with Frames?</summary></details>
<details><summary>What options do you have with animation on iOS?</summary></details>
<details><summary>How do you do animation with Frames and AutoLayout?</summary></details>
<details><summary>How do you work with UITableView?</summary></details>
<details><summary>How do you optimize table views performance for smooth, fast scrolling?</summary></details>
<details><summary>How do you work with UICollectionView?</summary></details>
<details><summary>How do you work with UIScrollView?</summary></details>
<details><summary>What is UIStackView? When would you use it and why?</summary></details>
<details><summary>What design patterns are commonly used in iOS apps?</summary></details>
<details><summary>What are SOLID principles? Can you give an example of each in iOS/Swift?</summary></details>
<details><summary>How do you manage dependencies in iOS applications?</summary></details>
<details><summary>What is Functional Programming and Functional Reactive Programming?</summary>
<img src="Lifecycle.png" width="301" height="400"> <img src="PushNotifications.png" width="301" height="400">
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

