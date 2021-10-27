# Functions - adder

## tl;dr

Get two whole numbers from the user, and then create an adder function to add the two numbers together.

Finally print your answer to the screen.

{% next %}

## Background

Functions are reusable sections of code that serve a articular purpose. Functions can take inputs and outpouts, and can be reused across programs.

Organizing programs into functions helps to organize and simplify code. This is an example of **abstraction**; after you have written the funtion, you can use the function without having to worry about the details of how the function is implemented.

---

Follow along and **TYPE** along with the instructions - **DO NOT copy and paste!!**

{% next %}

## Let's Start

Some of the code has been started for you, with comments telling you where to write most of your code.

You may need another header file to get your numbers from the user. If you can't remember, click on the hint.

{% spoiler "Hint" %}

This is the header file to use our `get` functions:

```c
#include <cs50.h>
```

{% endspoiler %}

{% next %}

## Get User Input

First things first, lets get some input from the user. Remember how we did this before? We will need two (2) whole numbers from the user. Let's name them `x` and `y`.

For this program, just assume the user will give you a whole number, no need to check!

{% spoiler "Hint" %}

First you will need to declare your variables, which are whole numbers or integers. Then we need to get the integers by using the function `get_int()`, and putting our prompt inside of the parentheses, inside of quotation marks.  Make sure that you leave a space to separate your prompt from the user input.

{% endspoiler %}

{% next %}

## Let's Add

First, you may want to create your adder function and put in your function declaration.

Then you will want to finish up `main`, calling your new function and then printing the answer to the screen.

{% spoiler "Click me for full program" %}

```c
#include <stdio.h>
#include <cs50.h>

int adder(int x, int y);

int main(void)
{
    // get integers from user
    int x = get_int("give me a whole number: ");
    int y = get_int("give me another whole number: ");
    
    //call adder function and pass in x and y
    int answer = adder(x, y);
    
    // print answer to screen
    printf("adding your nubmers together gives us: %i\n", answer);
}

int adder(int x, int y)
{
    return x + y;
}
```

{% endspoiler %}

{% next "Checks" %}

## Check Your Work

Be sure to `make` your program via the following:

```
make adder
```

Program won't make?

- Do you have all your semicolons (;) in place?
- Did you declare your variables correctly?
- Lastly, make sure to read the error messages, as they can help.

Then run your program via:

```
./adder
```

checking all conditions possible!

Not displaying correctly?

- Make sure you have the spacing correct in your prompts
- Make sure you put in the new line tags (\n)
