# Old Friends

## tl;dr

Improve upon older problems.

```
$ ./hello Milo
Hello, Milo!
$ ./fahrenheit 0
F: 32.0
$ ./pennies 28 1
$2684354.55
```

{% next %}

## Background

Here’s some good news for you right off the bat: you’ve seen almost everything we’re going to talk about in this problem once before. We’re going to revisit three old programs and rewrite them so that instead of taking input from the user while the program is running, they will instead accept input from the user at the command-line, before the program is even run.

You should see, in the window to the right, three files from programs we have previously done, including ```fahrenheit.c```, ```hello.c```, and ```pennies.c```. All you have to do is change the way that the user inputs data.

If you need, have a look at Doug’s short video on command-line arguments. Since we’ll be converting all three of the programs to accept command-line arguments (none of them currently do!), this video should come in handy.

{% video https://youtu.be/AI6Ccfno6Pk %}

If you happen to see (and are confused by!) ```char *``` in this and other shorts, know for now that ```char *``` simply means string. But more on that soon!

{% next %}

## Hello, again!

In Hello you were asked to write a program that very simply printed the message ```hello, world\n``` to the screen when run. It’s not too much of a leap to extend this program to say hello to a specific person by asking for the user to type a name at the prompt instead, so the program behaves like this.

```
~/chapter2/friends $ ./hello
Your name: Zamyla
hello, Zamyla
```

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

{% next "Submit" %}

## Submit

To submit `adder`, execute the below in the terminal window, logging in with your GitHub username and password when prompted. For security, you'll see asterisks (`*`) instead of the actual characters in your password.
```
submit50 candib80/cs50labs/c/adder
```
