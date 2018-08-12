# Swift-Observer-Design-Pattern
An Xcode 9 project, written in Swift 4, demonstrating how to implement the observer design pattern.

In this repo and [accompanying tutorial](), I explain the observer design pattern, where one instance, the _subject_, notifies (many) other instances, the _observers_, of changes to the state of the _subject_. The instances participating in this broadcast type communication don't need to know about one another. This is a great example of loose coupling. The subject instance, usually a single critical resource, broadcasts notifications about a change in its state to many observer instances that depend on that resource. Interested observers must subscribe to get notifications.

Here's the app -- resulting from building this project in Xcode -- in action:

![alt text][logo1]

[logo1]: http://iosbrain.com/wp-content/uploads/2018/08/ObserverAppDemo.gif "Observer"

## Xcode 9 project settings
**To get this project running on the Simulator or a physical device (iPhone, iPad)**, go to the following locations in Xcode and make the suggested changes:

1. Project Navigator -> [Project Name] -> Targets List -> TARGETS -> [Target Name] -> General -> Signing
- [ ] Tick the "Automatically manage signing" box
- [ ] Select a valid name from the "Team" dropdown
  
2. Project Navigator -> [Project Name] -> Targets List -> TARGETS -> [Target Name] -> General -> Identity
- [ ] Change the "com.yourDomainNameHere" portion of the value in the "Bundle Identifier" text field to your real reverse domain name (i.e., "com.yourRealDomainName.Project-Name").
