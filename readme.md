
# Commands Documentation

## Object Manipulation

### `object-you-want-to-reference:Destroy()`
- Description: Destroys an object.
- Syntax: `object-you-want-to-reference:Destroy()`

### `object-you-want-to-reference:connect(function)`
- Description: Adds a function to an object's stored functions.
- Syntax: `object-you-want-to-reference:connect(function)`

## System Commands

### `System:out/PrintIn("Text")`
- Description: Prints text to the system.
- Syntax: `System:out/PrintIn("Text")`

### `System:in/Flush()`
- Description: Removes all text from the console.
- Syntax: `System:in/Flush()`

### `System:in/Function(Functionname)`
- Description: Sandboxes a function by running it in the console instead of the main runtime.
- Syntax: `System:in/Function(Functionname)`

### `System:out/Function(Functionname)`
- Description: Removes a function from the console.
- Syntax: `System:out/Function(Functionname)`

### `System:in/code() { // body }`
- Description: Adds code to the console to be sandboxed.
- Syntax: `System:in/code() { // body }`

### `System:write(SystemFile, new data)`
- Description: Changes something about the VM for the language (use with caution).
- Syntax: `System:write(SystemFile, new data)`

## Canvas Commands

### `Canvas:new("name", x, y, width, height)`
- Description: Defines a new canvas.
- Syntax: `Canvas:new("name", x, y, width, height)`

### `Canvas:new ("name", x, y, width, height) { //body }`
- Description: Defines a new canvas and appends code to it.
- Syntax: `Canvas:new ("name", x, y, width, height) { //body }`

### `Canvas:out/PrintIn("Text")`
- Description: Adds text to an already defined canvas.
- Syntax: `Canvas:out/PrintIn("Text")`

### `Canvas:Destroy()`
- Description: Destroys a canvas.
- Syntax: `Canvas:Destroy()`

## Variable Handling

### Variable Creation
- Syntax: `new - var vartype name = value`

### Variable Assignment
- Syntax: `set - var name = value`

### Variable Increment
- Syntax: `change - name++`

### Variable Deletion
- Syntax: `delete - name:Destroy()`

### Variable Calling
- Syntax: `calling - name:return()`

### Referencing Object Syntax
- Syntax: `object/child/child/child/child`

## Defining Functions

### `Func return_type access_specifier name(parameters) [ // body ]`
- Description: Defines a function with a specified return type, access specifier, name, parameters, and body.
- Syntax: `Func return_type access_specifier name(parameters) [ // body ]`

## Loops

### `Looptype (LoopParameters) { // code }`

Available Looptypes and Parameters:
- "Times": "AmountToRepeat"
- "While": "Condition"
- "Until": "Condition"

## Variable Types

- Constant
- Mutable
- Private
- Public

Combinations:
- `mutable|private`
- `mutable|public`
- `constant|private`
- `constant|public`

---
