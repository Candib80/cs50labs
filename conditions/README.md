# Boolean Expressions & Conditions

## tl;dr

We will be getting two (2) numbers from the user and comparing them. Depending on our comparison, we will print a statement to the screen.

{% next %}

We will be practicing some Boolean expressions and conditions in this lab along with reinforcing what we have already been doing.

Follow along and TYPE along with the instructions - DO NOT copy and paste!!

{% next %}

## Let's Start

Make sure to put in your name and header file(s) as indicated in the `conditions.c` file to the right.

You will also need to begin your `main()` function.

If you can't remember the header files or how to start your `main()` function, read the hint.

{% spoiler "Hint" %}

Here's how we start every program:

```c
#include <stdio.h>
#include <cs50.h>

int main(void)
{

}
```

{% endspoiler %}

{% next %}

## Get User Input

First things first, lets get some input from the user. Remember how we did this before? We will need two (2) whole numbers from the user. Let's name them `x` and `y`.

{% spoiler "Hint" %}

Whole numbers are integers. We get integers by using the function `get_int()`, and putting our prompt inside of the parentheses, inside of quotation marks.  Make sure that you leave a space to separate your prompt from the user input.

{% endspoiler %}

{% next %}

## Let's Compare

For this next part we will be comparing `x` and `y`. If `x` is less than `y`, we are going to print as such. If `x` is greater than `y`, print this as well. Lastly the only other option is that `x` and `y` are equal.

- We use the `if`, `else if`, and `else` keywords to denote the forks in the road, based on Boolean expressions. `else` simply captures all the cases that haven’t fit into a previous condition.

- Note that curly braces, `{` and `}`, are used to wrap the lines of code that we want to run for each of the conditions if they are true. We also use indentation to make the lines of code more readable.

See if you can figure this out on your own before going forward.

{% next %}

Ok, so here is the code for our condition:

```c
if(x < y)
{
    printf("x is less than y\n");
}
else if(x > y)
{
    printf("x is greater than y\n");
}
else
{
    printf("x is equal to y\n");
}
```

{% next "Checks" %}

## Check Your Work

Be sure to `make` your program via the following:

```
make bool_conditions
```

Then run your program via:

```
./bool_conditions
```



---

{% next "Submit" %}

## Submit

Execute the below, logging in with your GitHub username and password when prompted. For security, you'll see asterisks (`*`) instead of the actual characters in your password.

```
submit50 cs50/2017/x/water
```
