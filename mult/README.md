# Functions, Command-line Arguments & Exit Codes - multiply

## tl;dr

Running the program with command-line arguments returns the product of the two whole numbers and prints the answer to the screen as per below. You should write a function to do the math portion.

```
./multiply 2 5
2 * 5 = 10
```

{% next %}

## Let's Start

Some of the code has been started for you, with comments telling you where to write most of your code.

## User Input

Ensure your user has entered the correct number of command-line arguments. How many should we have for this program?  
If the wrong number of arguments is entered, let the user know how they should use the program, via below, and exit the program.

```
Usage: ./multiply x y
```

You will also need to ensure that you convert the input from the command-line from a string to the proper data type.

{% spoiler "Hint" %}

Go back to `exit.c` from class or the Old Friends lab to see what we did to check for user input at the command line.

`argc` will be what we check to make sure the right number of arguments have been passed.

`atof()` or `atoi()` may be helpful here to convert data types. Remember to include the library that includes this function.

{% endspoiler %}

{% next %}

## Let's Multiply

First, you may want to create your multiply function and put in your function declaration (this goes between the `#includes` and `main`.

Then you will want to finish up `main`, calling your new function and then printing the answer to the screen.

{% spoiler "Click me for more help" %}

```c
#include <cs50.h>
#include <stdio.h>

int function(int x, int y); // function declaration

int main(int argc, string argv[])
{ 
    // check for correct number of arguments
    
    // call function and pass in x and y - this can be done in the next step instead of here
    
    // print answer to screen
    
}

int function(int x, int y)
{
    // body of your multiply function goes here
    // this will return the value of your variables after they are multiplied together
}
```

{% endspoiler %}

{% next "Checks" %}

## Check Your Work

Be sure to `make` your program via the following:

```
make multiply
```

Program won't make?

- Do you have all your semicolons (;) in place?
- Did you declare your variables correctly?
- Did you place your function declaration in the correct place?
- Lastly, make sure to read the error messages, starting with the one at the top, as they can help.

Then run your program via:

```
./multiply <x> <y>
```

checking all conditions possible!

Not displaying correctly?

- Make sure you have the spacing correct in your prompts
- Make sure you put in the new line tags (\n)
