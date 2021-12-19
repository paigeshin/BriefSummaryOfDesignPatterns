# Creational

### Builder

- Separate component for when object construction gets too complicated
- Can create mutually cooperating sub-builders
- Often has a fluent interface

### Factories

- Factory method more expressive than initializer
- Factory can be an outside class or inner class; inner class has the benefit of accessing private members

### Prototype

- Creation of object from an existing object
- Requires either explicit copying initializer or deep copy method

### Singleton

- When you need to ensure just a single instance eixsts
- Direct dependencies on a singleton are difficult to test (also difficult to refactor!)
- Consider extracting interface or using dependency injection

# Structural

### Adapter

- Converts the interface you get to the interface you need

### Bridge

- Decouple abstraction from implementation

### Composite

- Allows clients to treat individual objects and compositions of objects uniformly

### Decorator

- Attach additional responsibilities to objects
- “Inherit” from final classes or value types; emulate multiple inheritance

### Façade

- Provide a single unified interface over a set of interfaces

### Flyweight

- Space saving technique
- Efficiently support very large numbers of similar objects

### Proxy

- Provide a surrogate object that forwards calls to the real object while performing additional functions
- E.g., access control, communication, logging, etc.

# Behavioral

### Chain of Responsibility

- Allow components to process information/events in the chain
- Each element in the chain refers to next element; or
- Make a list and go through it

### Command

- Encapsulate a request into a separate object
- Good for audit, reply, undo/redo
- Part of CQS/CQRS (Query is also, effectively, a command)

### Interpreter

- Transform textual input into object-oriented structures
- Used by interpreters, compilers, static analysis tools, etc.
- Compiler Theory is a separate branch of Computer Science

### Iterator

- Provides an interface for accessing elements of an aggregate object
- Typically used implicitly via for...in..

### Mediator

- Provides mediation services between objects
- Objects not necessarily aware of each other’s presence
- E.g., message passing, chat room

### Memento

- Yields tokens representing system states
- Tokens do not allow direct manipulation, but can be used in appropriate APIs

### Observer

- Allows notification of listening components
- Uses the concept of an event
- Property observers built into the language

### State

- We model systems by having one of a possible states and transitions between these states
- Such a system is called a state machine
- Special frameworks exist to orchestrate state machines

### Strategy

- ‘Outsource’ part of an algorithm into separate implementations
- Can be selected at compile or runtime

### Template Method

- Define the outline of the algorithm with details filled in by inheritors

### Visitor

- Enable type-self traversal of data structures
- ‘Double dispatch’ requires each member of hierarchy to accept a visitor
