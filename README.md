# iOS-interview

## <a name='contents'>Table of Contents</a>

* [Cocoa touch](#cocoa-touch)
-----------
* [Memory Management](#memory-management)
* [Networking](#networking)
* [Multithreading](#multithreading)
* [Data persistance](#data-persistance)
* [Testing](#testing)
* [CoreAnimation, CoreGraphics, CoreText](#coreanimation-coregraphics-coretext)
* [Patterns(2,5,10)](#patterns)
* [Maps](#maps)
* [Swift](#swift)
* [Objective-C](#objective-c)
-----------
* [Code Puzzels](#code-puzzels)
* [Code](#code) 
-----------
* [General](#general)
-----------
* [HomeWork](#homework)
* [Podcasts](#podcasts)
* [Books](#books)
* [Job websites](#jobwebsites)
* [Companies](#companies)
* [Stories](#stories)
* [Process](#process)
* [Credits](#credits)

# Topics
1. Algorightms

1. Logical
2. Linked list
3. Arrays
4. Trees
5. Stacks
6. Recursion and dynamic programming
7. Bit manipulation
8. OoD
9. System design and scalability
10. Searching and Sorting
11. Testing
12. Threads
13. Databases
-leetcode, 2 alg books
-inter

- code/algorythms/knowledge

2. iOS code

Login system
Multithreading
CoreData

FizzBuzz
BinarySearch
ReverseLinkedList

-homeworks

3. iOS theory
-Class vs Struct

-networking
-testing
-arc, memory leaks, retain cycles
-Delegation and Observer/Notification
-view lifecycle
-filter, map, reduce
-Testing
-3D party libraries
-Gesture recogniser
-networking(Rest, Oauth2)
-debugging
-modulo 
-take home
-kvo 
-nsoperation vs multithreading
-Gcd 
-autolayout/sizeclasses
-nsnotification center
-UiView
-patterns of design
-github
-swiftbook
-optional biding 
-general expression
-question E, A, B, 50
-UIViewController
-notification center
-gcd, queues, operations

Networking rest
test
Google map kit
anotation
reverse geocoding
Location Manager
Algorithm design



## Cocoa touch 
[[⬆]](#contents)
autolayout

<details><summary>Name the framework that is used to construct application’s user interface for iOS. </summary>
The UIKit framework is used to develop application’s user interface for iOS. UIKit framework provides event handling, drawing model, windows, views, and controls specifically designed for a touch screen interface.
</details>
What is the diference between struct and class?
An  enum  is an object type whose instances represent  distinct  predefined  alternative values. Think of it as a list of known possibilities. An enum is the Swift way to express a set of constants that are alternatives to one another. An enum declaration includes case statements. Each case is the name of one of the alternatives. An instance of an enum will represent exactly one alternative — one case.

Methods A  method  is a function — one that happens to be declared at the top level of an object type declaration. This means that everything said about functions in  Chapter 2 applies. By default, a metho

Properties A  property  is a variable — one that happens to be declared at the top level of an object type declaration. This means that everything said about variables in  Chapter 3 applies. A property has a fixed type; it can be declared with  var  or  let; it can be stored or computed; it can have setter observers. An instance property can also be declared  lazy.

Structs A  struct  is the Swift object type  par excellence. An enum, with its fixed set of cases, is a reduced, specialized kind of object. A class, at the other extreme, will often turn out to be overkill; it has some features that a struct lacks, but if you don’t need those features, a struct may be preferable.

Classes A  class  is similar to a struct, with the following key differences: Reference type Classes are reference types. This means, among other things, that a class instance has two remarkable features that are not true of struct instances or enum instances: Mutability A class instance is mutable in place. Even if your reference to an instance of a class is a constant (let), you can change the value of an instance property through that reference. An instance method of a class never has to be marked  mutating  (and cannot be). Multiple references When a given instance of a class is assigned to multiple variables or passed as argument to a function, you get multiple references to  one and the same object. Inheritance A class can have a superclass. A class that has a superclass is a  subclass  of that superclass. Class types can thus form a hierarchical tree. In Objective-C, classes are the only object type. Some built-in Swift struct types are magically bridged to Objective-C class types, but your custom struct types don’t have that magic. Thus, when programming iOS with Swift, a primary reason for declaring a class, rather than a struct, is as a form of interchange with Objective-C and Cocoa.

Value Types and Reference Types A major difference between enums and structs, on the one hand, and classes, on the other, is that enums and structs are  value types, whereas classes are  reference types. A value type is  not mutable in place, even though it seems to be. For example, consider a struct. A struct is a value type:

What is let and var in Swift?
What is Optional in Swift and nil in Swift and Objective-C?
What are properties and instance variables in Objective-C and Swift?
What is a protocol (both Obj-C and Swift)? When and how is it used?
What is a category/extension? When is it used?
What are closures/blocks and how are they used?
What is MVC?
What are Singletons? What are they used for?
What is Delegate pattern in iOS?
What is KVO (Key-Value Observation)?
What does iOS application lifecycle consist of?
What is View Controller? What is its lifecycle?

What are the challenges in working with UI on iOS?
What do you use to lay out your views correctly on iOS?
What are CGRect Frames? When and where would you use them?
What is AutoLayout? When and where would you use it?
What are compression resistance and content hugging priorities for?
How does AutoLayout work with multi-threading?
What are the advantages and disadvantages of creating AutoLayouts in code versus using storyboards?
How do you work with storyboards in a large team?
How do you mix AutoLayout with Frames?
What options do you have with animation on iOS?
How do you do animation with Frames and AutoLayout?
How do you work with UITableView?
How do you optimize table views performance for smooth, fast scrolling?
How do you work with UICollectionView?
How do you work with UIScrollView?
What is UIStackView? When would you use it and why?
What alternative ways of working with UI do you know?
How do you make a pixel-perfect UI according to a designer’s specs?
How do you unit and integration test UI?
Step Seven: Beyond MVC. Design Pattens, Architecture, FRP, and Dependencies Management.
What design patterns are commonly used in iOS apps?
What is MVC?
What is MVVM?
What are the common layers of responsibility that an iOS application has?
What are SOLID principles? Can you give an example of each in iOS/Swift?
How do you manage dependencies in iOS applications?
What is Functional Programming and Functional Reactive Programming?
What are the design patterns besides common Cocoa patterns that you know of?

<img src="Lifecycle.png" width="301" height="400"> <img src="PushNotifications.png" width="301" height="400">
-UIApplicationDidFinishLaunching
-UIApplicationWillResignActive
-UIApplicationDidBecomeActive
-UIApplicationWillEnterForeground
-UIApplicationDidEnterBackground

viewDidLoad - update UI, outlets are set, bounds not set yet(no geometry)
viewWillApear - changing over display, geometry set, optimise performance,
viewDidApear - 
viewWillDisapear - remember whats going on and clean up, no time consuming
viewDidDisapear

viewWillLAyoutSubviews - called when frames changed
viewDidAyoutSubviews
viewWillTransition
didRecieveMemoryWarning
awakeFromNib

strong, weak, unowned

Closures
## Memory Management 
[[⬆]](#contents)

<details><summary>what is 'golden rule of memory management'? </summary></details> 
<details><summary>what is Arc?</summary></details>
<details><summary>what is Auto release pool?</summary></details>
<details><summary>Weak vs assign, strong vs copy?</summary></details>
<details><summary>Atomic vs nonatomic. What is the difference? How to change atomic/nonatomic setter in non ARC environment?</summary></details>
<details><summary>Why all properties reference to strong/retain?</summary></details>
<details><summary>What is NSCoder?</summary></details>

## Networking
[[⬆]](#contents)

<details> 
  <summary> Which JSON framework is supported by iOS?  </summary>
SBJson framework is supported by iOS.  It is a JSON parser and generator for Objective-C. SBJson provides flexible APIs and additional control that makes JSON handling easier.

</details>

<details> 
  <summary> Advantages and disadvantages of synchronous and asynchronous communication?</summary></details>
<details> 
  <summary> What does HTTP mean, TCP?</summary></details>
<details> 
  <summary> What are the differences between head, GET, post, put?</summary></details>
<details> 
  <summary> How do I download something from the Internet? What is the difference between synchronous and asynchronous requests? A little assignment. Describe how to download an image from the web and display it in imageview.g.h-all of this should happen after you click the button.</summary></details>
<details> 
  <summary> What is rest (restful)?</summary></details>
  <details> 
  <summary> What is json?</summary></details>
  
   <details> 
  <summary> What is NSCOder class used for? </summary>
  NSCoder is an abstractClass which represents a stream of data. They are used in Archiving and Unarchiving objects. NSCoder objects are usually used in a method that is being implemented so that the class conforms to the protocol. (which has something like encodeObject and decodeObject methods in them).</details>
  
   <details> 
  <summary>What's the difference between synchronous and asynchronous connections?</summary>
  Do not freeze the app, canceletion, authentication, it's impossible to parse data on the fly</details>
  
   <details> 
  <summary> Explain NSURLSession?</summary>
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
  <summary> Explain life cecle of URL Session?</summary>
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

  <details> 
  <summary>What is HTTP?
  <details> 
  <summary>What is REST?
  <details> 
  <summary>How do you typically implement networking on iOS?
  <details> 
  <summary>What are the concerns and limitations of networking on iOS?
  <details> 
  <summary>What should go into the networking/service layer?
  <details> 
  <summary>What is NSURLSession? How is it used?
  <details> 
  <summary>What is AFNetworking/Alamofire? How do you use it?
  <details> 
  <summary>How do you handle multi-threading with networking on iOS?
  <details> 
  <summary>How do you serialize and map JSON data coming from the backend?
  <details> 
  <summary>How do you download images on iOS?
  <details> 
  <summary>How would you cache images?
  <details> 
  <summary>How do you download files on iOS?
  <details> 
  <summary>Have you used sockets and/or pubsub systems?
  <details> 
  <summary>What is RestKit? What is it used for? What are the advantages and disadvantages?
  <details> 
  <summary>What could you use instead of RestKit?
  <details> 
  <summary>How do you test network requests?


## Multithreading 
[[⬆]](#contents)
<details> 
  <summary> Does iOS support multitasking? </summary>
iOS 4 and above supports multi-tasking and allows apps to remain in the background until they are launched again or until they are terminated.  
</details>


<details> 
  <summary> Why an app on iOS device behaves differently when running in foreground than in background? </summary>
An application behaves differently when running in foreground than in background because of the limitation of resources on iOS devices.
</details>

<details> 
  <summary> How can an operating system improve battery life while running an app? </summary>
An app is notified whenever the operating system moves the apps between foreground and background.  The operating system improves battery life while it bounds what your app can do in the background. This also improves the user experience with foreground app.
</details>

<details> 
  <summary> Which framework delivers event to custom object when app is in foreground? </summary>
The UIKit infrastructure takes care of delivering events to custom objects. As an app developer, you have to override methods in the appropriate objects to process those events.
</details>
LOOK

Queues
Main Queue
Global Queues 
DispatchQueue.global/main
queue.sync(async)

 a: if let url = URL(string: “http://stanford.edu/...”) {
 }
let task = session.dataTask(with: url) { (data: Data?, response, error) in // do something with the data
DispatchQueue.main.async {
// do UI stuff here
}
    print(“did some stuff with the data, but UI part hasn’t happened yet”)
b: c: d: e:
f:
g:
h: print(“done firing off the request for the url’s contents”)

## Data persistance 
[[⬆]](#contents)
### (CoreData)
<details> 
  <summary> What steps should be accomplish in order to save/fetch an object?  </summary>


</details>

What is the storage layer for in iOS applications?
What can you use to store data on iOS?
What is NSCoding?
What is NSUserDefaults?
What is Keychain and when do you need it?
How do you save data to a disk on iOS?
What database options are there for iOS applications?
How is data mapping important when you store data?
How would you approach major database/storage migration in your application?

How do access coredata?
NSManagedObjectContext

How do I you get contex?
NSPersistentContainer
(UIApplication.shared.delegate as! AppDelegate).persistentContainer

let container = (UIApplication.shared.delegate as! AppDelegate).persistentContainer let context: NSManagedObjectContext = container.viewContext

Every NSManagedObject knows the managedObjectContext it is in.

How do you access entities?
let context = AppDelegate.viewContext
  if let tweet = Tweet(context: context) {
tweet.text = “140 characters of pure joy”
tweet.created = Date() as NSDate
     let joe = TwitterUser(context: tweet.managedObjectContext)
     tweet.tweeter = joe
tweet.tweeter.name = “Joe Schmo” }

-Thread safety?
NSManagedObjectContext is not thread safe
Luckily, Core Data access is usually very fast, so multithreading is only rarely needed.
NSManagedObjectContexts are created using a queue-based concurrency model.
This means that you can only touch a context and its NSMO’s in the queue it was created on. Often we use only the main queue and its AppDelegate.viewContext, so it’s not an issue.
Thread-Safe Access to an NSManagedObjectContext context.performBlock { // or performBlockAndWait until it finishes
// do stuff with context (this will happen in its safe Q (the Q it was created on)) }
Note that the Q might well be the main Q, so you’re not necessarily getting “multithreaded.” It’s generally a good idea to wrap all your Core Data code using this.
Although if you have no multithreaded code at all in your app, you can probably skip it.
It won’t cost anything if it’s not in a multithreaded situation.

Convenient way to do database stuff in the background
The persistentContainer has a simple method for doing database stuff in the background AppDelegate.persistentContainer.performBackgroundTask { context in
// do some CoreData stuff using the passed-in context
// this closure is not the main queue, so don’t do UI stuff here (dispatch back if needed) // and don’t use AppDelegate.viewContext here, use the passed context
// you don’t have to use NSManagedObjectContext’s perform method here either
// since you’re implicitly doing this block on that passed context’s thread
try? context.save() // don’t forget this (and catch errors if needed)
}
This would generally only be needed if you’re doing a big update.
You’d want to see that some Core Data update is a performance problem in Instruments first. For small queries and small updates, doing it on the main queue is fine.

## Testing
[[⬆]](#contents)


<details><summary> Do you write unit tests? how you write in iOS?</summary></details>
<details><summary> What is TDD?</summary></details>
<details><summary> How TDD is good, and What problem does it solve?</summary></details>
<details><summary> What is Mocking, when you will use mocking?</summary></details>
<details><summary> What is UI testing?</summary></details>

<details><summary>Black or white box?</summary></details>
<details><summary>Who will use it and why?</summary></details>
<details><summary>What are the use cases?</summary></details>
<details><summary>What are the the bounds of use?</</summary></details>summary></details>
<details><summary>What are the failure conditions?

## CoreAnimation CoreGraphics CoreText 
[[⬆]](#contents)

## Patterns 
[[⬆]](#contents)

<img src="designpatterns1.jpg" width="301" height="400">
<img src="designpatterns2.jpg" width="301" height="400">

1. Singleton
2. Factory
3. Decorator
4. Builder
5. Proxy
6. Template
7. Adapter
8. Chain of Responsibility
9. Strategy
10. Flyweight
<details> 
  <summary>Explain Singleton class.</summary>
</details> 

<details> <summary>What is OOP?</summary></details>
<details> <summary>What are the pros and cons of inheritance?</summary></details>
<details> <summary>What is polymorphism?</summary></details>
<details> <summary>What is tight coupling?</summary></details>
<details> <summary>What are design patterns and how they are good?</summary></details>
<details> <summary>Tell me some important design patterns used in iOS?</summary></details>
<details> <summary>What is singleton?</summary></details>
<details> <summary>What challenges you have encounter implementing MVC?</summary></details>
<details> <summary>What is MVVM and why you will use it?</summary></details>
<details> <summary>What is dependency injection, how it is good?</summary></details>

1. MVC
2. Vapor
3. MVP
4. MVVC

https://www.youtube.com/watch?v=vNHpsC5ng_E&list=WL


* [Behavioral](#behavioral)
* [Creational](#creational)
* [Structural](#structural)

Behavioral
==========

>In software engineering, behavioral design patterns are design patterns that identify common communication patterns between objects and realize these patterns. By doing so, these patterns increase flexibility in carrying out this communication.
>
>**Source:** [wikipedia.org](http://en.wikipedia.org/wiki/Behavioral_pattern)

```swift

import Swift
import Foundation
```

👓 Observer
-----------

The observer pattern is used to allow an object to publish changes to its state.
Other objects subscribe to be immediately notified of any changes.

### Example

```swift

protocol PropertyObserver : class {
    func willChange(propertyName: String, newPropertyValue: Any?)
    func didChange(propertyName: String, oldPropertyValue: Any?)
}

final class TestChambers {

    weak var observer:PropertyObserver?

    private let testChamberNumberName = "testChamberNumber"

    var testChamberNumber: Int = 0 {
        willSet(newValue) {
            observer?.willChange(propertyName: testChamberNumberName, newPropertyValue: newValue)
        }
        didSet {
            observer?.didChange(propertyName: testChamberNumberName, oldPropertyValue: oldValue)
        }
    }
}

final class Observer : PropertyObserver {
    func willChange(propertyName: String, newPropertyValue: Any?) {
        if newPropertyValue as? Int == 1 {
            print("Okay. Look. We both said a lot of things that you're going to regret.")
        }
    }

    func didChange(propertyName: String, oldPropertyValue: Any?) {
        if oldPropertyValue as? Int == 0 {
            print("Sorry about the mess. I've really let the place go since you killed me.")
        }
    }
}
```

### Usage

```swift

var observerInstance = Observer()
var testChambers = TestChambers()
testChambers.observer = observerInstance
testChambers.testChamberNumber += 1
```

>**Further Examples:** [Design Patterns in Swift](https://github.com/kingreza/Swift-Observer)


Creational
==========

> In software engineering, creational design patterns are design patterns that deal with object creation mechanisms, trying to create objects in a manner suitable to the situation. The basic form of object creation could result in design problems or added complexity to the design. Creational design patterns solve this problem by somehow controlling this object creation.
>
>**Source:** [wikipedia.org](http://en.wikipedia.org/wiki/Creational_pattern)

```swift

import Swift
import Foundation
```

🌰 Abstract Factory
-------------------

The abstract factory pattern is used to provide a client with a set of related or dependant objects. 
The "family" of objects created by the factory are determined at run-time.

### Example
 
Protocols

```swift

protocol 

imal {
    func stringValue() -> String
    // factory
    static func make(string : String) -> Decimal
}

typealias NumberFactory = (String) -> Decimal

// Number implementations with factory methods

struct NextStepNumber: Decimal {
    private var nextStepNumber: NSNumber

    func stringValue() -> String { return nextStepNumber.stringValue }
    
    // factory
    static func make(string: String) -> Decimal {
        return NextStepNumber(nextStepNumber: NSNumber(value: (string as NSString).longLongValue))
    }
}

struct SwiftNumber : Decimal {
    private var swiftInt: Int

    func stringValue() -> String { return "\(swiftInt)" }
    
    // factory
    static func make(string: String) -> Decimal {
        return SwiftNumber(swiftInt:(string as NSString).integerValue)
    }
}
```

Abstract factory

```swift

enum NumberType {
    case nextStep, swift
}

enum NumberHelper {
    static func factory(for type: NumberType) -> NumberFactory {
        switch type {
        case .nextStep:
            return NextStepNumber.make
        case .swift:
            return SwiftNumber.make
        }
    }
}
```

### Usage

```swift

let factoryOne = NumberHelper.factory(for: .nextStep)
let numberOne = factoryOne("1")
numberOne.stringValue()

let factoryTwo = NumberHelper.factory(for: .swift)
let numberTwo = factoryTwo("2")
numberTwo.stringValue()
```

💍 Singleton
------------

The singleton pattern ensures that only one object of a particular class is ever created.
All further references to objects of the singleton class refer to the same underlying instance.
There are very few applications, do not overuse this pattern!

### Example:

```swift

class DeathStarSuperlaser {
    static let sharedInstance = DeathStarSuperlaser()

    private init() {
        // Private initialization to ensure just one instance is created.
    }
}
```

### Usage:

```swift

let laser = DeathStarSuperlaser.sharedInstance
 [Behavioral](Behavioral) |
 [Creational](Creational) |
 Structural
```

!!!!Builder
!!!!Factory Method

Structural
==========

>In software engineering, structural design patterns are design patterns that ease the design by identifying a simple way to realize relationships between entities.
>
>**Source:** [wikipedia.org](http://en.wikipedia.org/wiki/Structural_pattern)

```swift

import Swift
import Foundation
```

🍧 Decorator
------------

The decorator pattern is used to extend or alter the functionality of objects at run- time by wrapping them in an object of a decorator class. 
This provides a flexible alternative to using inheritance to modify behaviour.

### Example

```swift

protocol Coffee {
    func getCost() -> Double
    func getIngredients() -> String
}

class SimpleCoffee: Coffee {
    func getCost() -> Double {
        return 1.0
    }

    func getIngredients() -> String {
        return "Coffee"
    }
}

class CoffeeDecorator: Coffee {
    private let decoratedCoffee: Coffee
    fileprivate let ingredientSeparator: String = ", "

    required init(decoratedCoffee: Coffee) {
        self.decoratedCoffee = decoratedCoffee
    }

    func getCost() -> Double {
        return decoratedCoffee.getCost()
    }

    func getIngredients() -> String {
        return decoratedCoffee.getIngredients()
    }
}

final class Milk: CoffeeDecorator {
    required init(decoratedCoffee: Coffee) {
        super.init(decoratedCoffee: decoratedCoffee)
    }

    override func getCost() -> Double {
        return super.getCost() + 0.5
    }

    override func getIngredients() -> String {
        return super.getIngredients() + ingredientSeparator + "Milk"
    }
}

final class WhipCoffee: CoffeeDecorator {
    required init(decoratedCoffee: Coffee) {
        super.init(decoratedCoffee: decoratedCoffee)
    }

    override func getCost() -> Double {
        return super.getCost() + 0.7
    }

    override func getIngredients() -> String {
        return super.getIngredients() + ingredientSeparator + "Whip"
    }
}
```

### Usage:

```swift

var someCoffee: Coffee = SimpleCoffee()
print("Cost : \(someCoffee.getCost()); Ingredients: \(someCoffee.getIngredients())")
someCoffee = Milk(decoratedCoffee: someCoffee)
print("Cost : \(someCoffee.getCost()); Ingredients: \(someCoffee.getIngredients())")
someCoffee = WhipCoffee(decoratedCoffee: someCoffee)
print("Cost : \(someCoffee.getCost()); Ingredients: \(someCoffee.getIngredients())")
```

🎁 Façade
---------

The facade pattern is used to define a simplified interface to a more complex subsystem.
(REST api)

### Example

```swift

enum Eternal {

    static func set(_ object: Any, forKey defaultName: String) {
        let defaults: UserDefaults = UserDefaults.standard
        defaults.set(object, forKey:defaultName)
        defaults.synchronize()
    }

    static func object(forKey key: String) -> AnyObject! {
        let defaults: UserDefaults = UserDefaults.standard
        return defaults.object(forKey: key) as AnyObject!
    }

}
```

### Usage

```swift

Eternal.set("Disconnect me. I’d rather be nothing", forKey:"Bishop")
Eternal.object(forKey: "Bishop")
```


## Maps 
[[⬆]](#contents)

<details> 
  <summary>How to implement uimapkit in the app?</summary></details>






## Swift
[[⬆]](#contents)

<details><summary>What is Class?</summary></details>
<details><summary>What is Object?</summary></details>
<details><summary>What is Interface?</summary></details>
<details><summary>What is Struct? What differs from an Object Type?</summary></details>
<details><summary>Communication ways between classes?</summary></details>
<details><summary>Delegate, Notification, KVO?</summary></details>
<details><summary>When do you use each one of these?</summary></details>
<details><summary>Working with Threads?</summary></details>
<details><summary>NSOperationBlock, Grand Central Dispatcher, Thread</summary></details>
<details><summary>Explain strong, assign, retain, weak ?</summary></details>
<details><summary>Garbage Collector on iOS? How it works on iOS?</summary></details>
<details><summary>What is Container View Controller?</summary>
UITabBarController, UINavigationController, UISplitViewController, Child view controllers and siblings.</details>

<details><summary>What is UIStackView?</summary></details>
<details><summary>What are the states of an iOS App?</summary>
There are five : Not Running, Inactive, Active, Background, Suspended </details>
<details><summary>What does code signing do?</summary></details>
<details><summary>What is the difference between property and  instance variable?</summary>
Simply, property is public, instance variable is private.</details>
<details><summary>what is  Deadlock? </summary></details>
<details><summary>what is Weak? </summary></details>
<details><summary>what is Strong? </summary></details>
<details><summary>what is Unowned? </summary></details>
<details><summary>what is Leaking, dangling? </summary></details>

<details><summary>what is Class, struck, enam? </summary>three flavors of object type</details>
<details><summary>what is Oop? </summary></details>
<details><summary>what is Mvp? </summary></details>
<details><summary>what is reserved word?</summary></details>
<details><summary>what is Inout? </summary></details></summary></details>
<details><summary>what is Anonymous function(omission)? </summary></details>
<details><summary>what is the difference between category, extension and protocol? </summary></details>

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



## Objective-C 
[[⬆]](#contents)

<details><summary> What is the difference between underscore and self (i.e self.xx and _xx) ?</summary></details>
<details><summary> What is property?</summary></details>
<details><summary> What is the difference between weak and strong?</summary></details>
<details><summary> What is Retain Cycle? And how we can avoid it?</summary></details>
<details><summary> What does copy means while declaring a property?</summary></details>
<details><summary> What is synthesize and when we need to use it?</summary></details>
<details><summary> What is a category?</summary></details>
<details><summary> What is an extension?</summary></details>
<details><summary> How we can add a property in a category?</summary></details>
<details><summary> What is method swizzling and when we should use it?</summary></details>
<details><summary> How we can layout subviews in a view?</summary></details>
<details><summary> What are the size classes?</summary></details>
<details><summary> What is ARC?</summary></details>
<details><summary> What is @autorelease and when we should use it?</summary></details>
<details><summary> How to animate view with constraint?</summary></details>
<details><summary> What is core data?</summary></details>
<details><summary> What is core data stack?</summary></details>
<details><summary> What is managed object context?</summary></details>
<details><summary> How we can do multithreading with core data?</summary></details>
<details><summary> How to transfer manage object from one thread to another thread?</summary></details>
<details><summary> How to merge changes from one moc to another?</summary></details>
<details><summary> Difference between bounds and frame?</summary></details>
<details><summary> What does dispatch_once do?</summary></details>
<details><summary> What is delegate?</summary></details>
<details><summary> How we can do multithreading in iOS?</summary></details>
<details><summary> When you will use NSOperations over GCDs and vice versa?</summary></details>
<details><summary> What does alloc do?</summary></details>
<details><summary> How we can create a class in objective c which don’t inherit from NSObject?</summary></details>
<details><summary> What are the different application states in iOS?</summary></details>
<details><summary> How we can execute some code when app is in background?</summary></details>
<details><summary> How we can wait for some thread to finish before starting another?</summary></details>
<details><summary> How you will store user info (username, password or token) securely in iOS?</summary></details>





<details> 
  <summary> Name the framework that is used to construct application’s user interface for iOS</summary>
In addition to the core app behaviors, UIKit provides support for the following features
</details>
 <details> 
  <summary>Whats a struct? </summary>
A struct is a special C data type that encapsulates other pieces of data into a single cohesive unit. Like an object, but built into C. </details>

<details> 
  <summary>
What are the different ways to specify layout of elements in UIView?</summary>
Here are a few common ways to specify the layout of elements in UIView:
• Using InterfaceBuilder, you can add a XIB file to your project, layout elements within it, and then load the XIB in your application code (either automatically, based on naming conventions, or manually). Also, using InterfaceBuilder you can create a storyboard for your application.
</details>

<details> 
  <summary>Can outlet be static?</summary>
  </details>

<details> 
  <summary>How would you implement static blur effect to the UIView subclass to make it work fast (as of iOS 6-7 it was a problem)  </summary>
  </details>



<details> 
  <summary>What is the difference between atomic and non-atomic properties? Which is the default for synthesized properties? When would you use one over the other?</summary>
  </details>

<details> 
  <summary>Does Objective-C contain private methods?</summary>
NO, there is nothing called a private method in Object-C programming. If a method is defined in .m only then it becomes protected. If in .h,it is public.
If you really want a private method then you need to add a local category/ unnamed category/ class extension in the class and add the method in the category and define it in the class.m</details>

<details> 
  <summary>What is plist?</summary>
Plist refers to Property lists that organize data into named values and lists of values using several object types. These types provide you the means to produce data that is meaningfully structured, transportable, storable, and accessible, but still as efficient as possible. Property lists are frequently used by applications running on both Mac OS X and iOS. The property-list programming interfaces for Cocoa and Core Foundation allow you to convert hierarchically structured combinations of these basic types of objects to and from standard XML. You can save the XML data to disk and later use it to reconstruct the original objects.
The user defaults system, which you programmatically access through the NSUserDefaults class, uses property lists to store objects representing user preferences. This limitation would seem to exclude many kinds of objects like as NSColor and NSFont objects, from the user default system. But if objects conform to the NSCoding protocol they can be archived to NSData objects, which are property list–compatible objects</details>

<details> 
  <summary>What is the purpose of reuseIdentifier? </summary>
  </details>
  
 <details> 
  <summary> What is the benefit of setting it to a non-nil value?</summary>
  </details>

<details> 
  <summary>What is the difference between an “app ID” and a “bundle ID” and what is each used for?</summary>
Since most users consider the App ID as string, they think it is interchangeable with Bundle ID. Once the App ID is created in the Member Center, you can only use the App ID Prefix that matches the Bundle ID of the Application Bundle.
The bundle ID uniquely defines each App. It is specified in Xcode. A single Xcode project can have multiple targets and therefore, output multiple apps. A common use case for this – An app having both lite/free and pro/full versions or branded multiple ways.</details>

<details> 
  <summary>What is Abstract class in Cocoa?</summary>
Cocoa doesn’t provide anything called abstract. We can create a class abstract that gets checked only at runtime while it is not checked at compile time.
@interface AbstractClass : NSObject
@end
@implementation AbstractClass
+ (id)alloc{
    if (self == [AbstractClass class]) {
        NSLog(@"Abstract Class can’t be used");
    }
    return [super alloc];
@end</details>

<details> 
  <summary>What is NSURLConnection class? Define its types and use case.</summary>
There are two ways of using NSURLConnection class. One is asynchronous and the other is synchronous.
An asynchronous connection will create a new thread and performs its download process on the new thread. A synchronous connection will block the calling thread while downloading content and doing its communication.
Many developers think that a synchronous connection blocks the main thread, which is not true. A synchronous connection will always block the thread from which it is fired. If you fire a synchronous connection from the main thread, the main thread will be blocked. But, if you fire a synchronous connection from a thread other than the main thread, it will be like an asynchronous connection and won’t block your main thread.
In fact, the only difference between a synchronous and an asynchronous connection is that at runtime, a thread will be created for the asynchronous connection while it won’t do the same for a synchronous connection.
In order to create an asynchronous connection, we need to do the following:
1. Have our URL in an instance of NSString
2. Convert our string to an instance of NSURL
3. Place our URL in a URL Request of type NSURLRequest, or in the case of mutable URLs, in an instance of NSMutableURLRequest.
4. Create an instance of NSURLConnection and pass the URL request to it.</details>

<details> 
  <summary>What is the relation between iVar and @property?</summary>
iVar is an instance variables. It cannot be accessed unless we create accessors, which are generated by @property. iVar and its counterpart @property can be of different names.
@interface Box : NSObject{
    NSString *boxName;
}
@property (strong) NSString *boxDescription;//this will become another ivar
-(void)aMethod;
@end
@implementation Box
@synthesize boxDescription=boxName;//now boxDescription is accessor for name
-(void)aMethod {
    NSLog(@"name=%@", boxName);
     NSLog(@"boxDescription=%@",self.boxDescription);
    NSLog(@"boxDescription=%@",boxDescription); //throw an error
}
@end</details>

<details> 
  <summary>
What happens if IApplication object does not handle an event?
</summary>
In such case the event will be dispatched to your app delegate for processing.</details>

<details> 
  <summary>
Name the framework that is used to construct application's user interface for iOS?
</summary>
The UIKit framework is used to develop application's user interface for iOS. UIKit framework provides event handling, drawing model, windows, views, and controls specifically designed for a touch screen interface.</details>

<details> 
  <summary>
How is the app delegate is declared by Xcode project templates?
</summary>
App delegate is declared as a subclass of UIResponder by Xcode project templates.</details>

<details> 
  <summary>
How can you respond to state transitions on your app?
</summary>
On state transitions can be responded to state changes in an appropriate way by calling corresponding methods on app's delegate object.

For example:
application Did Become Active method can be used to prepare to run as the foreground app.
application Did Enter Background method can be used to execute some code when app is running in the background and may be suspended at any time.
application Will Enter Foreground method can be used to execute some code when your app is moving out of the background application Will Terminate method is called when your app is being terminated.</details>

<details> 
  <summary>
When an app is said to be in active state?
</summary>
An app is said to be in active state when it is running in foreground and is receiving events.</details>

<details> 
  <summary>
Assume that your app is running in the foreground but is currently not receiving events. In which sate it would be in?
</summary>
An app will be in InActive state if it is running in the foreground but is currently not receiving events. An app stays in InActive state only briefly as it transitions to a different state.</details>

<details> 
  <summary>
Give example scenarios when an application goes into InActive state?
</summary>
An app can get into InActive state when the user locks the screen or the system prompts the user to respond to some event e.g. SMS message, incoming call etc.</details>

<details> 
  <summary>
List down apps state transitions when it gets launched?
</summary>
Before the launch of an app, it is said to be in not running state.
When an app is launched, it moves to the active or background state, after transitioning briefly through the inactive state.</details>

<details> 
  <summary>
Who calls the main function of you app during the app launch cycle?
</summary>
During app launching, the system creates a main thread for the app and calls the app's main function on that main thread. The Xcode project's default main function hands over control to the UIKit framework, which takes care of initializing the app before it is run.</details>

<details> 
  <summary>How can you respond to state transitions on your app?</summary>
State transitions can be responded to state changes in an appropriate way by calling corresponding methods on app’s delegate object.
For example:
applicationDidBecomeActive( ) method can be used to prepare to run as the foreground app.
applicationDidEnterBackground( ) method can be used to execute some code when app is running in the background and may be suspended at any time.
applicationWillEnterForeground( ) method can be used to execute some code when your app is moving out of the background
applicationWillTerminate( ) method is called when your app is being terminated.</details>

<details> 
  <summary>What is the difference between retain & assign?</summary>
Assign creates a reference from one object to another without increasing the source’s retain count.
if (_variable != object)
{   
 [_variable release];  
  _variable = nil;  
  _variable = object;
 }
Retain creates a reference from one object to another and increases the retain count of the source object.
if (_variable != object)
{
  [_variable release];
    _variable = nil;  
_variable = [object retain];  
}</details>

<details> 
  <summary>
Whats fast enumeration?
</summary>
Fast enumeration is a language feature that allows you to enumerate over the contents of a collection. (Your code will also run faster because the internal implementation reduces
message send overhead and increases pipelining potential.)</details>
<details> 
  <summary>
What is iphone sdk?
</summary>
iPhone SDK is available with tools and interfaces needed for developing, installing and running custom native applications.
Native applications are built using the iPhone OS’s system frameworks and Objective-C language and run directly on iPhone OS.
Native applications are installed physically on a device and can run in presence or absence of network connection.</details>

<details> 
  <summary>
What is an iPhone app?
</summary>
An iPhone app is a program that runs on our iPhone/iPod Touch. It enables us to ccomplish a certain task. They could be utility apps, games, enterprise apps, entertainment apps, apps to access our bank account etc.</details>
<details> 
  <summary>
What is iphone architecture?
</summary>
It is similar to MacOS X architecture
It acts as an intermediary between the iPhone and iPod hardware an the appearing applications on the screen
The user created applications never interact directly with the appropriate drivers, which protects the user applications from changes to the hardware.</details>

<details> 
  <summary>
Introduction to Iphone application Development?
</summary>
In 2007, Apple entered the cellular phone business with the introduction of the iPhone, a multi-touch display cell phone, which also includes the features of iPod.</details>

<details> 
  <summary>
What is iphone reference library?
</summary>
iPhone reference library is a set of reference documents for iPhone OS .
It can be downloaded by subscribing to the iPhone OS Library doc set.
Select Help>Documentation from Xcode, and click the subscribe button next to the iPhone OS Library doc set, which appears in the left column.</details>

<details> 
  <summary>
How many bytes we can send to apple push notification server.?
</summary>
256bytes.</details>

<details> 
  <summary>
What are sensors in iphone?
</summary>
The proximity sensor immediately turns off the display when the iPhone is lifted to ear. With this sensor the power is saved and accidental dialing is prevented.
The display is automatically brightens the iPhone by the ambient light sensor when the sunlight or bright rooms and dims in darker places.</details>




<details> 
  <summary>
Which object manage the presentation of apps content on the screen?
</summary>
View controller objects takes care of the presentation of app's content on the screen. A view controller is used to manage a single view along with the collection of subviews. It makes its views visible by installing them in the app's window.</details>

<details> 
  <summary>
How to change the content of your app in order to change the views displayed in the corresponding window?
</summary>
To change the content of your app, you use a view controller to change the views displayed in the corresponding window. Remember, window itself is never replaced.</details>

<details> 
  <summary>
Difference between shallow copy and deep copy?
</summary>
Shallow copy is also known as address copy. In this process you only copy address not actual data while in deep copy you copy data.
Suppose there are two objects A and B. A is pointing to a different array while B is pointing to different array. Now what I will do is following to do shallow copy.
Char *A = {‘a','b','c'};
Char *B = {‘x','y','z'};
B = A;
Now B is pointing is at same location where A pointer is pointing.Both A and B in this case sharing same data. if change is made both will get altered value of data.Advantage is that coping process is very fast and is independent of size of array.
while in deep copy data is also copied. This process is slow but Both A and B have their own copies and changes made to any copy, other will copy will not be affected.</details>

<details> 
  <summary>
Which app specific objects store the apps content?
</summary>
Data model objects are app specific objects and store app's content. Apps can also use document objects to manage some or all of their data model objects.</details>

<details> 
  <summary>
Name the application thread from where UIKit classes should be used?
</summary>
UIKit classes should be used only from an application's main thread. Note: The derived classes of UIResponder and the classes which manipulate application's user interface should be used from application's main thread.</details>

<details> 
  <summary>
What are the location services?
</summary>
Applications such as Maps, camera and compass are allowed to use the information from cellular, Wi-Fi and Global Positioning System networks for determining the approximate locations.
The location is displayed on the screen, using a blue marker.</details>


<details> 
  <summary>
Describe the functionality of accelerometer of an iphone
</summary>
iPhone responds to motion using a built-in accelerometer.
The accelerometer detects the movement and changes the display accordingly, at the time of rotating iPhone from portrait to landscape.</details>
<details> 
  <summary>
Where can you test Apple iPhone apps if you don't have the device?
</summary>
iOS Simulator can be used to test mobile applications. Xcode tool that comes along with iOS SDK includes Xcode IDE as well as the iOS Simulator. Xcode also includes all required tools and frameworks for building iOS apps. However, it is strongly recommended to test the app on the real device before publishing it.</details>


<details> 
  <summary>What are the features added in iOS 5?</summary>
  </details>
  
  <details> 
  <summary>What are the features added in iOS 6?</summary>
  </details>
  
  <details> 
  <summary>What are the features added in iOS 7?</summary>
  </details>
  
  <details> 
  <summary>What are the features added in iOS 8?</summary>
  </details>
  
<details> 
  <summary>What are the features added in iOS 9?</summary>
• Intelligent Search and Siri- Intelligent Search is an excellent mechanism to learn user habits and act on that information- open apps before we need them, make recommendations on places we might like and guide us through our daily lives to make sure we’re where we need to be at the right time.
Siri is a personal assistant to the users, able to create contextual reminders and search through photos and videos in new ways. Swiping right from the home screen also brings up a new screen that houses “Siri Suggestions,” putting favorite contacts and apps right on your fingertips, along with nearby restaurant and location information and important news.
</details>

<details> 
  <summary>What are the features added in iOS 10?</summary>
  
  
</details>

<details> 
  <summary>Explain Singleton class.</summary>
Only one instance of that class is created in the application.
@interface SomeManager : NSObject
             + (id)singleton;
 @end
 @implementation SomeManager
            + (id)singleton {    
                                 static id sharedMyManager = nil; 
                                 @synchronized([MyObject class]){ 
                                                     if (sharedMyManager == nil) { 
                                                                         sharedMyManager = [[self alloc] init]; 
                                                      } 
                                 }
                                return sharedMyManager;
            }
 @end
//using block
+ (id) singleton {
    static SomeManager *sharedMyManager = nil;
    static dispatch_once_t  onceToken;
    dispatch_once(&onceToken, ^{
        sharedMyManager = [[self alloc] init];
    });
    return sharedMyManager;</details>
    
    


## Code Puzzels 
[[⬆]](#contents)
### Whiteboard
1. https://www.hackerrank.com/
2. https://leetcode.com/
3. https://coderpad.io/
4. www.codingame.com


### Data structures
1. Linked Lists
2. Trees, Tries, Graphs
<details><summary>Given two linked lists, find the node at which they merge.</summary></details> 
<details><summary>Given an n x n grid, find the number of ways to get from the bottom left to the top right given that you can only move up or right each time and you cannot move to any node on the bottom diagonal half of the grid, i.e. row less than col.  </summary></details>
3. Stacks & Queues 
4. Heaps
5. Vectors / ArrayLists
6. Hash Tables 
7. LOGICAL
<details><summary>
“Suppose you are in a hallway lined with 100 closed lockers. You begin by opening all 100 lockers. Next, you close every second locker. Then you go to every third locker and close it if it is open or open it if it’s closed — call this toggling the lockers. You continue toggling every nth locker on pass number n. After your hundredth pass of the hallway, in which you toggle only locker number 100, how many lockers are open?”</summary></details>
<details><summary>
Domino's 64-2 </summary></details>
<details><summary>
5 boxes and a black cat</summary></details>

### Algorythms
1. Breadth-First Search
2. Depth-First Search
3. Binary Search
4. Merge Sort
5. Quick Sort
6. Insert Search
7. Bucket Sort
8. Selection Sort
9. Bubble Sort
10. Radix Sort
11. Sparse Search
12. Topologic Sort
13. Dijkstra's algorithms
14. Red black trees LogN
15. In order Traversal
16. Hashtable collision(LL/Binary search tree/open addressing with probing/quadratic probing and double hashing
17. Rabin-Karp substring search 
18. AVL trees 
19. In-order traversal
20. Pre-order traversal 
21. Strassen's Algorithms 

### Concepts
1. Bit Manipulation
2. Memory(Steack vs Heap)




## Code 
[[⬆]](#contents)

<details> 
  <summary>UIPanGestureRegogniser</summary></details>


## General
[[⬆]](#contents)

<img src="interview.png" width="301" height="100">
<details> 
  <summary>
Why should we hire you?</summary>
life way</details>
How is success in this position measured and rewarded?
How are the goals for this job set?
What would I be expected to accomplish in the first 6 months?
How long have you been with the company?

<details> 
  <summary>Tell me about company from cv?</summary></details>
<details> 
  <summary>tell me what did you do there and about app?</summary></details>
<details> 
  <summary>your responsibilities?</summary></details>
<details> 
  <summary>How did you do “patterns of design”?</summary></details>
<details> 
  <summary>How did you write your code?</summary></details>
<details> 
  <summary>How did you write tests?</summary></details>
<details> 
  <summary>Give an example of your work situation?</summary>
examples from work “Long loading, where did I implement creativity”
</details>

<details> 
  <summary>Tell about yourself?</summary></details>
<details> 
  <summary>What is your biggest achievement?</summary></details>
<details> 
  <summary>why should we hire you?</summary></details>
<details> 
  <summary>What value you can bring?</summary></details>
<details> 
  <summary>How would you rank your knowledge in points from 0 to 10?</summary></details>
  
<details> 
  <summary>  Why are you interested in this field?</summary></details>
<details> 
  <summary>Why are you interested in this company?</summary></details>
<details> 
  <summary>Why are you interested in this position?</summary></details>

<details> 
  <summary>What is your greatest weakness?</summary></details>
<details> 
  <summary>What is your lack of related experience?</summary></details>
<details> 
  <summary>Why your GPA is so low?</summary></details>
<details> 
  <summary>Do you have lack of leadership experiences?</summary></details>
<details> 
  <summary>What is your record of job-hopping?</summary></details>
  
<details> 
  <summary> Name 3 of your favorite mobile apps</summary>

If you’ve chosen App Developing as a career, chances are you’re always in the know of the latest apps. The recruiting manager will expect you are always trying out and testing different apps and you have a solid criteria about what’s well done and what should improve. Be sure you take some of your favorite apps on your smartphone, be prepared to talk about them from functionality and developing context.
</details>

<details> 
  <summary>How do you handle security issues?</summary>

Security is always a very delicate subject especially when talking about mobile devices.  Show your knowledge about security and expose your ideas about how to minimize security issues in the app they are creating. Get informed, was there a recent attack to a specific type of software? Mention it and be prepared to explain how you would have solved it.</details>

<details> 
  <summary>What’s the importance of user interface/user experience (UI/UX) in mobile application development?</summary>

User interface and user experience are key to successful mobile applications, so expect a lot of UI/UX questions. State your opinions and tips on getting the most out of the mobile’s interface. You may point out which apps you think have a great UI and which ones don’t. Also, some recruiters may ask you to quickly draw a scheme of an interface –be prepared to do it.</details>

<details> 
  <summary>Do you have any experience migrating an app from one platform to another?</summary>

Most apps must be available on more than one OS, so experience reconfiguring or migrating an app from one platform to another is a very valuable treat. Tell about your experience in this field and detail the apps you have reconfigured and the solutions you have found to do it. If you don’t have any experience, expose the reasons why you think you are technically prepared to do it.</details>


<details> 
  <summary>What is you main disadvantage?</summary>
There are two types of disadvantages
one we can controll, there is one and we are aware about it
the other one, there is a disadv, but we are not aware about it
Help me to find faults
And very grateful

I have a shortage
but! We are fighting
Preodalival in the past and what are the disadvantages of today, when I know that there is a defect I'm working on
Details and says no and priorities and took it to the end</details>

<details> 
  <summary>How would you describe your perfect day</summary></details>
<details> 
<summary>What is good code practices?</summary>
Good code practices
Variables names
Long method 
Cellid rav value create constant 
Less print statements 

Apple convention
Braces and names camelCase

The Routine is the enemy of time it is flying by
</details>

Tell me about your previous Job?
STAR technique
What was the main advanteges
problem
how did you solve it

Tell me about the time when you failed/succeeded?
Tell me something what is not on your CV?
What do you do for fun?
Tell me about your leadership example?
Tell me about the time you worked on a team?
Tell me about your favourite project?

### Question(my)
What is normal day look like?
Why did you choose this company?


## HomeWork 
[[⬆]](#contents)

https://github.com/dmyma/UnifyID_MalashenkoDmytro

MiniProjects
url - https://www.youtube.com/watch?v=aTj0ZLha1zE&list=WL&index=2
tap - 

## Podcasts 
[[⬆]](#contents)
### Youtube
1. https://www.youtube.com/user/SiliconValleyVoice/playlists
2. https://www.youtube.com/user/letsbuildthatapp
3. https://www.youtube.com/user/SeanAllan
### iTunes
2. https://itunes.apple.com/hk/podcast/sharedinstance/id967705766?mt=2
3. https://itunes.apple.com/hk/podcast/more-than-just-code-podcast-podcast-about-ios-os-x/id906987516?mt=2
4. https://itunes.apple.com/hk/podcast/consult/id1018251429?mt=2
5. https://itunes.apple.com/hk/podcast/fatal-error/id1139051496?mt=2
6. https://itunes.apple.com/hk/podcast/free-agents/id1138055739?mt=2
7. https://itunes.apple.com/hk/podcast/swift-unwrapped/id1209817203?mt=2
8. https://itunes.apple.com/hk/podcast/under-the-radar/id1055685246?mt=2
### APPS
1.  iOS Interview
### SITES
1. raywenderlich.com
2. Indie iOS Focus Weekly
3. iosGoodies
4. ios Cookies
5. CocoaControl
6. appcode
## Books
[[⬆]](#contents)
1. Objective-C
2. Swift from apple
3. Design Patterns
4. Algorithms
5. Cracking Code interview

## Job websites 
[[⬆]](#contents)

1. www.dice.com
2. www.glassdoor.com
3. angel.co 
4. upwork.com
5. international hr

## Companies
[[⬆]](#contents)

italki.com
EPAM.com
amazon.com

google.com
apple.com

## Cities
1. San Francisco 14
2. Boston
3. San Diego
4. Minneapolis
5. LA
6. NY
7. Seattle
8. Austin/Phoenix -8
9. Sacramento
9.1 Orlando/Porttland
10. Cleveland -22

## Stories 
[[⬆]](#contents)

1. https://habrahabr.ru/post/285680/
2. https://medium.freecodecamp.com/how-i-learned-to-code-and-earned-a-job-in-silicon-valley-changing-my-life-along-the-way-a3af854855fa
3. https://medium.freecodecamp.com/how-i-left-my-consulting-career-behind-and-broke-into-tech-36ea0c1a0407

## Process 
meate project - OS -Freelance
[[⬆]](#contents)
192-17-5-6-3-1(6 weeks)0.52%
26-15-6-5-2-  (8 weeks)
2500h-70p-1500c-20000l
2h-2ti
d, Mac, app, sf

<details> 
  <summary>Step 1: send CV</summary>
</details> 
  
<details> 
  <summary>Step 2: phone screening</summary>
  Go on site for sreening and if it is good you can get HW
  - Background, experience - typical recruiter call. 

</details> 


<details> 
  <summary>Step 2.5: technical phone screen.</summary>
</details> 

<details> 
  <summary>Step 3: Technical interview/whiteboard</summary>
  -whiteboard code
  -iOS frameworks OOP DesignP DataStrcu Algorithm
  -patterns
  -arhitecture
  -technical 
  -Think of a product - it could be anything. What features do you like about it? What would you improve, and how?  

</details> 

<details> 
  <summary>Step 4: Home work </summary>
  1. https://www.interviewbit.com/
  2. https://www.hackerrank.com/
  3. https://www.topcoder.com/
  4. www.codingame.com
</details> 

<details> 
  <summary>Step 5: on site 4-8 hours with 4-8 people</summary>
</details> 

## Credits 
[[⬆]](#contents)

1. http://www.geekinterview.com/Interview-Questions/iOS
2. http://way2ios.com/development/ios-development-2/ios-interview-questions-with-answers/
3. https://www.linkedin.com/groups/121874/121874-6146133293344579586
4. https://medium.com/ios-os-x-development/50-ios-interview-questions-and-answers-part-2-45f952230b9f
5. https://github.com/ochococo/Design-Patterns-In-Swift#creational
6. https://github.com/soapyigu/LeetCode_Swift/blob/master/README.md
7. https://github.com/9magnets/iOS-Developer-and-Designer-Interview-Questions#general
8. https://github.com/durul/My-Medium-Articles
9. https://github.com/5uper0/ios-science
10. http://www.geekinterview.com/Interview-Questions/iOS
11. github.com
12. google
13. raywanderlich


