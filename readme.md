---

# S.P.A.R.C. documentation

## Introduction

S.P.A.R.C. is a powerful and versatile language designed for adding to game engines. It combines a clear syntax with a rich set of features to enable efficient and expressive programming. This guide will walk you through the various aspects of the language, including syntax, commands, object manipulation, system functions, and more.

## Syntax Overview

### Defining Functions

Syntax: `Func return_type access_specifier name(parameters) [ // body ]`

- `Func`: Keyword to define a function.
- `return_type`: Specifies the return type of the function (e.g., `void`, `int`, `string`).
- `access_specifier`: Determines the visibility of the function (`public`, `private`, etc.).
- `name`: Name of the function.
- `parameters`: Input parameters for the function.
- `body`: Code block containing the function's logic.

Example:
```sparc
Func void public MyFunction(int param) [
    // Function body
]
```

### Commands

Syntax: `referencingobject.commandname(parameters)`

- `referencingobject`: Refers to the object or entity the command operates on.
- `commandname`: Name of the command to execute.
- `parameters`: Input parameters required by the command.

Example:
```sparc
myObject:Destroy()
System:out/PrintIn("Hello, world!")
```

### Variables

Syntax: `var vartype name = value`

- `var`: Keyword to declare a variable.
- `vartype`: Type of the variable (`int`, `string`, `boolean`, `mutable`, `constant`, `public`, `private`).
- `name`: Name of the variable.
- `value`: Initial value assigned to the variable.

Example:
```sparc
var int myNumber = 10
var string myString = "Hello"
```

### Loops

Syntax: `Looptype (LoopParameters) { // code }`

- `Looptype`: Type of loop (`Times`, `While`, `Until`).
- `LoopParameters`: Conditions or parameters for the loop.
- `code`: Code block to be executed repeatedly.

Examples:
```plaintext
Times (10) {
    // Code to repeat 10 times
}

While (x < 100) {
    // Code to repeat while condition is true
}
```

### System Commands

Syntax: `System:commandname(parameters)`

- `System`: Keyword to access system-related commands.
- `commandname`: Name of the system command to execute.
- `parameters`: Input parameters required by the command.

Example:
```Sparc
System:in/Flush()
System:in/Function(MyFunction)
```

### Canvas Commands

Syntax: `Canvas:commandname(parameters)`

- `Canvas`: Refers to commands related to canvas manipulation.
- `commandname`: Name of the canvas command.
- `parameters`: Input parameters required by the command.

Example:
```sparc
Canvas:new("myCanvas", 0, 0, 800, 600)
Canvas:out/PrintIn("Text")
```

## Key Concepts

### Object Manipulation

- Objects can be created, manipulated, and destroyed using specific commands (`object:command(parameters)`).
- Commands can be connected to objects to extend their functionality (`object:connect(function)`).

### Functions and Control Flow

- Functions are defined using the `Func` keyword and can have specified return types and access specifiers.
- Loops (`Times`, `While`, `Until`) and conditional statements (`If`, `Else`, `Switch`) control program flow.

### System Functions

- System commands (`System:command(parameters)`) provide access to system-level functionalities like console manipulation and function sandboxing.

### Canvas Handling

- Canvas commands enable the creation and manipulation of graphical canvases, allowing for interactive visual elements in applications.

### Variable Management

- Variables can be declared with specific types (`int`, `string`, etc.) and can be manipulated using assignment, incrementing, and deletion operations.

## Conclusion

S.P.A.R.C. offers a robust set of features for developing diverse applications, from console-based utilities to graphical interfaces. By mastering its syntax and understanding its key concepts, developers can create efficient and scalable software solutions.

