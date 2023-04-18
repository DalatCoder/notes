
# Uml and Object-Oriented Design Foundations

<a href="https://udemy.com/course/uml-and-object-oriented-design-foundations" target="_blank">Course</a>

Why study UML?

- Mastering a programming language is not enough
- Be able to design a software system
- Understand and apply OO-principles
- Describe your design using a standard language
- UML - common diagramming techniques
- Used at many companies and enterprises

UML course overview

- Software development methodologies
- Fundamental object orientation concepts
- Object oriented design
- UML basics
- Fundamental diagram types
- Case study: designing a note taking app

Tools and prerequisites

- Beginner-friendly
- staruml.io

## Some terms:

- Spaghetti code: complicated, difficult to understand and maintain
- Variable: value with a type identified using a name
- Data structure: a way of organizing data in a computer program
- UML: Unified modeling language - graphical notation used to describe object-oriented systems
- User story: very brief description of a feature
- Epic: describe a bigger chunk of functionality. Should be split into smaller user stories.

## Traditional and Agile software development

### What are software development methodologies?

There are different ways to develop a software system.
Sure, you can just sit down and start typing source code.
This works until, well, it doesn't. For anything more complicated than a "Hello world" app, you will need
a way to organize your work.
And if you're not working alone, the lack of a reasonably well defined process is going to lead to
chaos.

As the complexity of a project and the number of involved people increases, the need for a development
process becomes more and more prevalent.
Different approaches have been invented to solve this situation.
We're going to talk about two of the most popular development methodologies, namely: The Waterfall model,
which requires you to have a detailed plan before starting any coding.
The requirements need to be fixed, so no changes are expected during development.
And the second one is the change friendly, responsive, Agile approach, which works great for projects
where the expectations can change rapidly and frequently.

Now, before we dive into these methodologies, I must tell you one thing.
None of these systems can precisely describe every step of the software development process, but we
definitely need them to synchronize and organize our development related activities - activities that
include not only coding, but also design, product management, budgeting, testing, documentation,
release and maintenance.

### The waterfall model

### The agile approach

## Core object orientation concepts

### A brief history of programming

Programming paradigms:

- 1950: non-structured programming
  - sequentially ordered instructions
  - numbered code lines

```sinclair
10 PRINT "Fahrenheit", "Celsius"
20 PRINT
30 INPUT "Enter degree F", F
40 PRINT F, (F-32) * 5/9
50 GO TO 30
```

- 1960: structured programming
  - logical steps
  - relies on subroutines: contain a set of instructions to be carried out
  - improves code readability
  - reduces development time

- 1980: object oriented programming
  - split apart the program into self-contained objects
  - an object acts as a program
  - an object operates on its own data
  - each object interacts with other objects

### Objects

- OOP is organized around objects
- properties
- identity: their own state
- behavior: their own behavior

### Classes

We need a class to create objects. The class is the blueprint of an object.
You can think of a class as a plan, a description of what an object will be.

class:
- name
- properties
- methods

### Abstraction

Abstraction is a way of describing complex problems in simple terms by ignoring some details. It helps
us focus on the bigger picture. We can dig deeper once we have a broder understanding.

### Encapsulation and data hiding

Data hiding: avoid exposing the inner workings of our objects.

When designing your classes, expose only as much detail as needed.

Data hiding plays an essential role in keeping the dependencies between objects to a minimum.
A tightly-coupled system, with most of the objects depending on each other is an obvious 
sign of a bad design. Updating or maintaning such a system is a pain.
Any tiny modification will cascade down and require you to change other parts
of the system, too.

### Inhertitance

Code reuse.

Object orientation is about granularity and separation of concerns.
Each class should focus on a set of specific functionalities and do that well.
Creating one-size-fits-all monolithic classes is a major mistake and object-oriented software development.

### Polymorphism

- polys: many, much
- morphe: form, shape

polymorphism: the condition of occurring in several different forms

Method overriding: subclasses can provide a specialized implementation of a method defined in the superclass.

## Object oriented analysis and design

### Fundamental object oriented analysis and design concepts

Building an object oriented application requires some prelimianary steps. These steps are similar regardless
of the development methodology.

- 1. collect requirements:
  - identify the problems we want to solve
  - clarify the functionality required to solve the problems
  - document important decisions

- 2. describe the software:
  - describe the system from the user's point of view
  - create wireframes and prototypes if needed

- 3. identify the classes
- 4. create diagrams using UML

### Collecting requirements

Requirement means "a thing that is needed or wanted". We must clarify what's needed or wanted in our application.
The features of the system are the so-called functional requirements.

Functional requirements:
- Represent the features
- Define how to react to an input
- Determine the expected behavior

Non-functional requirements:
- Not directly related to the features of the system
- Performance
- Legal requirements
- Documetation
- In form: `<The app/system> must <do something>` 

Requirements collection: define what the system needs to do. Identify constraints and boundaries.

### Mapping requirements to technical descriptions

Decribe the system from the user's point of view.

- Use case:
  - Title: short, descriptive use case title ("create a new trip", "add expense", "convert currencies")
  - Actor: user
  - Scenario: explain how the software works in this sceraio

Example

- Create new trip
- Actor: mobile user
- Scenario:
  - The suer can initiate the creation of a new trip from the main screen
  - The title is mandatory. All the other settings are optional
  - Optionally, the user can write a short description and set a start and end date for the trip
  - The app assigns a default home currency based on the phone's settings. Users can override
    the default home currency with any of the supported currencies
  - the app allows setting a budget for the trip. This setting is optional
  - Also, the user can assign a custom thumbnail to a trip
  - The user can save the trip or cancel the trip creation process

Avoid technical terms.

User stories are another common way of describing certain features or parts of our application.
User stories are shorter than use case descriptions, usually only one to two sentences long.

User stories format: `As a <type of user>, I want <some goal> so that <some reason>`. 

Example: 
- As a user, I want to add notes to my expenses, so that I can identify them later on.
- As a power user, I want to retrieve the app's database file, so that I can inspect it on any computer.

If you can't describe the user story in one or two sentences, you may need to split it into multiple smaller user stories.

The larger user stories are known as `epics`.

### Why do we need a common descriptive language?

UML diagrams: standard graphical notation used to describe object-oriented systems.


