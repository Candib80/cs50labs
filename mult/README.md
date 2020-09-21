# Functions - multiply

## tl;dr

Get two whole numbers from the user, and then create a function to multiply the two numbers together.

Finally print your answer to the screen.

{% next %}

## Let's Start

Some of the code has been started for you, with comments telling you where to write most of your code.

## Get User Input

First things first, lets get some input from the user. Remember how we did this before? We will need two (2) whole numbers from the user. Let's name them `x` and `y`.

For this program, just assume the user will give you a whole number, no need to check!

{% spoiler "Hint" %}

First you will need to declare your variables, which are whole numbers or integers. Then we need to get the integers by using the function `get_int()`, and putting our prompt inside of the parentheses, inside of quotation marks.  Make sure that you leave a space to separate your prompt from the user input.

Your code will look similar to this:

```c
variable = get_int("prompt: ");
```

{% endspoiler %}

{% next %}

## Let's Multiply

First, you may want to create your mulitply function and put in your function declaration (this goes between the `#includes` and the `main`.

Then you will want to finish up `main`, calling your new function and then printing the answer to the screen.

{% spoiler "Click me for more help" %}

```c
#include <stdio.h>
#include <cs50.h>

int function(int x, int y); // functions declaration

int main(void)
{
    // get integers from user
    
    //call function and pass in x and y - this can be done in the next step instead of here
    
    // print answer to screen
    
}

int function(int x, int y)
{
    //body of your mulitply function goes here
    //this will return the value of your variables after they are multiplied together
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
- Lastly, make sure to read the error messages, starting with the one at the top, as they can help.

Then run your program via:

```
./multiply
```

checking all conditions possible!

Not displaying correctly?

- Make sure you have the spacing correct in your prompts
- Make sure you put in the new line tags (\n)

{% next "Submit" %}

## Submit

To submit `multiply`, execute the below in the terminal window, logging in with your GitHub username and password when prompted. For security, you'll see asterisks (`*`) instead of the actual characters in your password.
```
submit50 candib80/cs50labs/c/mult
```
