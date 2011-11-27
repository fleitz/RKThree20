RestKit Three20 Integration
---------------------------

This project provides integration between the [RestKit framework](http://restkit.org/) and
Facebook's [Three20 framework](http://three20.info/) via the TTModel interface. TTModel is 
an Objective-C protocol used to coordinate activities between a data source and a Three20
table controller. The bindings within RKThree20 allow the use of a RestKit object loader to
drive a Three20 table view.

## Installation
1. Add RestKit to your project. Installation instructions are available at: https://github.com/RestKit/RestKit/wiki/Installing-RestKit-in-Xcode-4.x
1. Add Three20 to your project. Installation instructions are available at: http://three20.info/article/2010-10-06-Adding-Three20-To-Your-Project
1. Check out the RKThree20 project into the same directory you have the Three20
and RestKit sources within your project. They should be siblings within the directory structure
of your project. For example, if you keep all of your libraries within a **Libraries** directory, 
then you should have `Libraries/three20`, `Libraries/RestKit`, and `Libraries/RKThree20`. This is important
because the project is configured with cross-project references that assume that RestKit and Three20 live
at ../ in the containing project.
1. Drag **RKThree20.xcodeproj** onto your project to create a cross-project reference.
1. Configure a target dependency on the **RKThree20.a** library so that it is built with your project.
1. Link the **RKThree20.a** library into your project.
1. Import the RKThree20 headers: `#import <RestKit/Three20/Three20.h>`

## Usage
Leveraging RKThree20 requires an understanding of both the RestKit and Three20 frameworks. The best available documentation for RKThree20 is available by reading the code of the [RKDiscussionBoard](https://github.com/RestKit/RKDiscussionBoard) example project.

## Status
This library was removed from the main RestKit codebase and is not supported. Patches and documentation are welcome, but the RestKit team is not actively developing the module.