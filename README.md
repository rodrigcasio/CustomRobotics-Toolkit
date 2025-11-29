# Custom Robotics Toolkit (C++)

This is a small C++ project I made to practice using templates and basic C++ programming. The program creates a simple toolkit with functions that can work with different types of data (like integers, doubles, and strings) using templates. I wanted to build this as a toolkit for robotics lab work, where they can handle different data types without needing to repeat the code.

## What does it do?

- **Creates template functions** that can work with different data types (int, double, string) without writing separate code for each type.
- **Provides utility functions** like finding the midpoint between two numbers and swapping values.
- **Uses a template class** called `DataHolder` that can store and manage different types of data with min/max limits.
- **Shows how templates work** by demonstrating the same functions working with integers, doubles, and strings.
- **Prints the results** to the console, so you can see how templates handle different data types.

## Example Output

When you run the program, you'll see output like this:

```
Result (int): 30
Result (double): 2.9815
---
"firstNumber" new value: 18
"secondNumber" new value: 7
---
"greeting" new value: world
"planet" new value: hello
---
Current value from first test is 21
New value: 78
Current value is: 100
---
The current value of the string stored is: robotics lab
---
	=== ToolKit Demo ===
The mid point of 1000 - 3000 is: 2000
----
"part1" new value is: engine
"part2" new value is: alpha
----
The special number value is: 3.9
----
The name of the robot is: CASIONATOR THE DESTROYER
	=== End of ToolKit Demo ===
```

## Why did I make this?

I wanted to practice using templates in C++ and understand how to write code that can work with different data types. I also wanted to build this as a toolkit for robotics lab work, where they often need to handle different types of data (sensor readings, coordinates, robot names, etc.) without writing separate code for each type. This project helped me learn how templates make code more flexible and reusable, and how to create template classes that can handle different types of data efficiently.

## How to Run

This project uses **CMake** build system generator for easy, cross-platform compilation. Follow these steps from the root directory of the project `CustomRobotics-Toolkit/`

1. **Ensure CMake is installed:**
- Make sure you have CMake (version 3.1- or higher please) and a C++ compiler (g++ or clang++) installed on your system.

2. **Generate the build system (configure):**
- Create a separated directory for the build files  and run CMake inside it. Keeping source files clean

```bash
mkdir build
cd build
cmake ..
```

3. **Build:**
- Use generated build system (`make` on Unix-like systems) to compile the executable.

```bash 
make
```

4. **Run the program:**
- The executable (RoboticsToolkit) will be placed inside the `build` directory.

```bash 
./RoboticsToolkit
```

**IMPORTANT: Note for windows users:**

- Windows developers have two ways to build the project using CMake.
  - **Command line (MSYS2/Cygwin):** If you use an environment like **MSYS2** or **WLS** (Windows Subsystem for Linux), you can follow the **Standard Build** steps above exactly.
  - **Visual Studio:** CMake can generate a Visual Studio solution. Run CMake from your `developer command prompt`, specify the generator:

```bash 
cmake .. -G "Visual Studio 17 2022"
```

Then, open the generated `.sln` file and build within Visual Studio IDE.

## Author

Rodrigo Casio  
[My GitHub Profile](https://github.com/rodrigcasio)
