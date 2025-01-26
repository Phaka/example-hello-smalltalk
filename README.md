# Smalltalk Hello World Example

A minimal Smalltalk implementation of "Hello, World!" that demonstrates the language's elegant object-oriented design. This example shows how in Smalltalk, everything - even string literals - is a fully capable object that can receive messages.

## Understanding the Simplicity

Our implementation is just one line:

```smalltalk
'Hello, World!' printNl.
```

This single line demonstrates several profound ideas that influenced modern programming:

1. Everything is an object: The string 'Hello, World!' is not just data - it's a full-fledged object that can receive messages.

2. All computation is message passing: We don't call a function named print - instead, we send the message printNl to our string object.

3. Uniform access: There's no distinction between "primitive" types and objects. A string literal can receive messages just like any other object.

The period at the end isn't just punctuation - it's a message terminator that tells Smalltalk where one message expression ends and another begins.

## Running the Program

You can run this program using GNU Smalltalk:

### Linux and macOS
```bash
gst hello.st
```

### Windows (via WSL)
```bash
gst hello.st
```

## Historical Context

This simple example embodies Alan Kay's original vision for object-oriented programming. When Kay coined the term "object-oriented," he wasn't thinking about classes and inheritance - he was thinking about independent objects communicating through messages. Our one-line program shows exactly that: a string object receiving a message to print itself.

The directness of `'Hello, World!' printNl.` contrasts sharply with other languages:

- C: `printf("Hello, World!\n");` - Calls a function on data
- Java: `System.out.println("Hello, World!");` - Accesses a static field before printing
- Python: `print("Hello, World!")` - Calls a function on a string
- Smalltalk: `'Hello, World!' printNl.` - Sends a message to an object

The Smalltalk version is arguably the most conceptually pure - there's just an object and a message.

## Installing GNU Smalltalk

### Linux
On Debian/Ubuntu:
```bash
sudo apt update
sudo apt install gnu-smalltalk
```

On Fedora:
```bash
sudo dnf install gnu-smalltalk
```

### macOS
Using Homebrew:
```bash
brew install gnu-smalltalk
```

### Windows
GNU Smalltalk can be built from source on Windows, but it's recommended to use WSL (Windows Subsystem for Linux) and follow the Linux installation instructions.

## Why This Matters

While our first version with a Hello class and main method would work, it brought unnecessary complexity from other programming traditions. The one-line version better demonstrates Smalltalk's revolutionary idea that everything is an object that responds to messages. This concept influenced many modern languages:

- Ruby's design was heavily influenced by Smalltalk's message passing
- Objective-C's message syntax was directly inspired by Smalltalk
- JavaScript's prototype-based object system shares ideas with Smalltalk
- Modern fluent interfaces and method chaining echo Smalltalk's message passing

## Further Reading

- "Smalltalk-80: The Language and its Implementation" (The Blue Book) - Adele Goldberg
- [GNU Smalltalk Manual](https://www.gnu.org/software/smalltalk/manual/html_node/index.html)
- "The Early History Of Smalltalk" by Alan Kay - Explains the thinking behind Smalltalk's design
