# ZebraOPSYSIta-Eng
Overview
Zebra Base Operating System (Zebra OS) is an experimental and simple command-line-based operating system simulation, designed to showcase basic memory management and register editing operations. Currently in its alpha stage (version 0.3), it allows users to edit registers and memory, perform basic arithmetic operations, and store values temporarily or permanently.

The project is still in an early stage, with plans to expand functionality in future versions.

Features
Register Editing: Modify values in the program’s register system using regedit().
Memory Editing: Modify memory slots using memoryedit().
Basic Arithmetic Operations: Perform addition and subtraction via sum() and sub().
Storage Viewing: View both memory and register data using showstorage().
Help System: Get documentation for all available functions with help().
Safe Exiting: Exit the program safely using quit().
Functions Overview
1. regedit(pos, value)
Allows you to modify a specific position in the register.
Example usage:

python
Copy code
regedit(0, True)
2. memoryedit(pos, value)
Edits the memory at the specified position.
Example usage:

python
Copy code
memoryedit(1, 42)
3. sum(a, b, do)
Performs the sum of a and b. Depending on the value of do, the result can be printed, saved temporarily, or saved permanently in memory.
Options for do:

"print": prints the result
"savetemp": stores the result in sumVAR temporarily
"saveperm": saves the result in memory
Example usage:

python
Copy code
sum(3, 5, "print")
4. sub(a, b, do)
Subtracts b from a. Similar options for do as with the sum() function.

Example usage:

python
Copy code
sub(10, 4, "saveperm")
5. showstorage(arg1)
Displays either the memory or the register based on the argument.
Options for arg1:

"mem" or "memory": displays the memory
"reg" or "register": displays the register
Example usage:

python
Copy code
showstorage("memory")
6. quit()
Exits the program safely and displays a message.

7. help()
Displays a list of available functions and their purpose.

Installation & Usage
Prerequisites
Python 3.x installed on your machine.
Running the Program
Clone or download this repository.
Open a terminal or command prompt and navigate to the project directory.
Run the Python script:
bash
Copy code
python3 zebra_os.py
Follow the on-screen prompts to interact with the system.
Example Workflow
Run the program.
When prompted, enter the name of the function you want to execute (e.g., sum).
Enter any required positional and keyword arguments as requested by the program.
Planned Features for Future Versions
Persistent memory: In future releases, memory will be persistent across sessions.
Additional arithmetic operations: Multiplication, division, and more.
User-defined memory slots: Allow users to dynamically define memory size and positions.
Error handling improvements: More robust handling of incorrect inputs and exceptions.
License
(c) 2024 GEA Innovations Studio. All rights reserved.

Author
Developed by GEA Innovations Studio.

