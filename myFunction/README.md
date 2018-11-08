# myFunction

## tl;dr

Be creative and make your own program with a function...

Keep reading before coding!

{% next %}

## Let's Start

In the `myFunction.c` file to the right, create a program of your choosing using the following requirements:
  
  - You must get at least one input from the user (this can be a number or a string)
  - You must create at least one function and use it in main
    - This function can either return a value, or create a side effect (look at the CS50 Reference sheet to figure out the difference if you don't remember)
    
 Your program need not be complicated, but use your imagination to create something!

{% spoiler "User Input Hint" %}

First you will need to declare your variables, with their type. 

Then we need to get the user input by using the function `get_int()` `get_string()` or the like, and putting our prompt inside of the parentheses, inside of quotation marks.  Make sure that you leave a space to separate your prompt from the user input.

Your code will look similar to this, but keep in mind how yours will change if you are getting a string or a different kind of number:

```c
variable = get_int("prompt: ");
```

{% endspoiler %}

{% spoiler "Click me to see program structure" %}

```c
#include <stdio.h>
#include <cs50.h>
//depending upon your program, you may need other header files

// function declaration will go here instead of this comment

int main(void)
{
    // the main part of your program goes here
    // put in relevent comments as you go
    
}

returnType functionName(parameters)
{
    //body of your function goes here
}
```

{% endspoiler %}

{% next "Checks" %}

## Check Your Work

Be sure to `make` your program via the following (ensuring to capitalize where needed):

```
make myFunction
```

Program won't make?

- Do you have all your semicolons (;) in place?
- Did you declare your variables correctly?
- Lastly, make sure to read the error messages, as they can help.

Then run your program via:

```
./myFunction
```

checking all conditions possible!

Not displaying correctly?

- Make sure you have the spacing correct in your prompts
- Make sure you put in the new line tags (\n)

{% next "Submit" %}

## Submit

Submit via the command-line by typing the following:

`submit50 functions/myFunction@candib80/checks`
