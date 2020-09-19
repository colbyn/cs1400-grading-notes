# An alternative -more elaborate- explanation

In a manner of speaking, computation is about data and algorithms that operate on such data. Though this will vary depending on the nature of your program. 

For this question you will consider your program to be a ‘black box’ (so to speak), and therein consider how the outside world interacts with your program, and how your program interacts with the outside world. Furthermore consider the aforementioned interactions to be your program’s inputs and outputs respectively, and thereafter write down these inputs and outputs using the following format. 

For simple CLI based programs that run as batch processes, use **two tables** to define all the inputs and outputs of your program.

Regarding the tables, there will be three columns:
1. The name; obviously printing e.g. “Hello world” won’t have a formal name, but assign it some name, in the same manner as you would name a variable. 
2. The type. Some additional notes:

    * For the overly meticulous: On Unix like systems, printing to the console and writing to some arbitrary file use the same underlying APIs. Printing “hello world” simply writes to a special file handle called `stdout` or sometimes `stderr`. Obviously printing e.g. “Hello world” won’t have a formal type, but if you assigned “Hello world” to some variable, what would the resulting type be? Likewise if the output is a file, don’t consider the output type to be ‘file handle’, but the value that is being written to the file. Consider ‘file handle’ to be an implementation specific detail that this question isn’t concerned about. Furthermore if you are writing numeric values to a given file handle, obviously this value will (either explicitly or implicitly) be serialized to a string prior to writing to the given file, but again consider this serialization to be an implementation specific detail, instead consider the type of the value prior to such. 

    * The purpose of this column is to get you accustomed to thinking about what types your variables will manifest at runtime.

3. Some example value.

## Format Example

1. Entering [...] and [...] for [...] results in [...] printed to the console and the termination of the program with a non-zero exit code.
2. Entering [...] for [...] and [...] for [...] results in [...] and [...]
3. The program should output a non-empty file named [...]