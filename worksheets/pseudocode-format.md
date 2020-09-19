# Pseudocode Format

For the worksheet assignments, the expected pseudocode format should be something akin to an ordered list, analogous to the sequential order in which your actual code will be executed at runtime. 

E.g.
```
1. Do X.
2. Do Y.
3. Do Z. 
… 
```


**Remember, don’t use sentences, mathematical formulas, or python code.**
Don’t simply use newlines to denote individual instructions, use an ordered list (which may be nested if appropriate). 

## Example

Here is an example for a simple script that prompts the user for some inputs, computes a summary value, and prints out the results.

### Good

1. Get the number of [...] from user
1. Get the number of [...] from user
2. Convert [...] to ints
3. Check for [...]
4. Check for [...]
5. Compute [...] for each [...]
6. Compute [...] for [...]
7. Compute [...] from [...]
8. Compute [...] from remaining [...]
9. Print out [...] following the formatting specifications



The above is just an example, especially the given format. For instance, instead of this format:
> Get the number of [...] from user

Can could have written:
> Prompt the user for the number of [...]


### Bad

<div style="border: 1px solid #262626">
<p>Get the number of [...] from user</p><br/>
<p>Get the number of [...] from user</p><br/>
<p>Convert [...] to ints</p><br/>
<p>Check for [...]</p><br/>
<p>Check for [...]</p><br/>
<p>Compute [...] for each [...]</p><br/>
<p>Compute [...] for [...]</p><br/>
<p>Compute [...] from [...]</p><br/>
<p>Compute [...] from remaining [...]</p><br/>
<p>Print out [...] following the formatting specifications</p>
</div>

Regarding the above, don’t simply use newlines to denote individual instructions, use an ordered list (which may be nested if appropriate). 


<hr/>

# An alternative -more elaborate- explanation

In a manner of speaking, computation is about data and algorithms that operate on such data. Though this will vary depending on the nature of your program. 

For this question you will consider your program to be a ‘black box’ (so to speak), and therein consider how the outside world interacts with your program, and how your program interacts with the outside world. Furthermore consider the aforementioned interactions to be your program’s inputs and outputs respectively, and thereafter write down these inputs and outputs using the following format. 

For simple CLI based programs that run as batch processes, use **two tables** to define all the inputs and outputs of your program.

Regarding the tables, there will be three columns:
1. The name; obviously printing e.g. “Hello world” won’t have a formal name, but assign it some name, in the same manner as you would name a variable. 
2. The type. Some additional notes:

    2.1. On Unix like systems, printing to the console and writing to some arbitrary file use the same underlying APIs. Printing “hello world” simply writes to a special file handle called `stdout` or sometimes `stderr`. 
    2.2. Obviously printing e.g. “Hello world” won’t have a formal type, but if you assigned “Hello world” to some variable, what would the resulting type be? Likewise if the output is a file, don’t consider the output type to be ‘file handle’, but the value that is being written to the file. Consider ‘file handle’ to be an implementation specific detail that this question isn’t concerned about. Furthermore if you are writing numeric values to a given file handle, obviously this value will (either explicitly or implicitly) be serialized to a string prior to writing to the given file, but again consider this serialization to be an implementation specific detail, instead consider the type of the value prior to such. 
    2.3. The purpose of this column is to get you accustomed to thinking about what types your variables will manifest at runtime.

3. Some example value.


<hr/>


Hope this helps! 
