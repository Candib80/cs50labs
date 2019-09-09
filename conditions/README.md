# Boolean Expressions & Conditions

## tl;dr

We will be getting two (2) numbers from the user and comparing them. Depending on our comparison, we will print a statement to the screen.

We will be practicing some Boolean expressions and conditions in this lab along with reinforcing what we have already been doing.

{% next %}

## Background

**Conditions** are how programmers can make decisions in programs, by allowing some parts of the code to only run under certain circumstances. Conditions will generally work by evaluating a **boolean expression**, which is an expression that will have a value of either `true` or `false`. Programmers can set conditions such that different code will run depending on what the value of the boolean expression is.

Boolean operators are used to create boolean expressions that evaluate to `true` or `false`. Common boolean operators include the comparison operators: `<` (less than), `>` (greater than), `==` (equal to), `<=` (less than or equal to), `>=` (greater than or equal to), and `!=` (not equal to). 

Logical operators can also be used to combine boolean expressions. `&&` is the logical AND operator: it will evaluate to `true` if both expressions on either side of it are true. `||` is the logical OR operator: it evaluates to `true` if at least one of the two expressions on either side is true. And `!`, the logical NOT operator, evaluates to the opposite of whatever the expression immediately after it is.

---

Follow along and **TYPE** along with the instructions - **DO NOT copy and paste!!**

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

First you will need to declare your variables, which are whole numbers or integers. Then we need to get the integers by using the function `get_int()`, and putting our prompt inside of the parentheses, inside of quotation marks.  Make sure that you leave a space to separate your prompt from the user input.

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
make conditions
```

Program won't make?

- Do you have all your semicolons (;) in place?
- Did you declare your variables correctly?
- Lastly, make sure to read the error messages, as they can help.

Then run your program via:

```
./conditions
```

checking all conditions possible!

Not displaying correctly?

- Make sure you have the spacing correct in your prompts
- Make sure you put in the new line tags (\n)

{% next "Submit" %}

## Submit

Submit via the command-line by typing the following:

submit50 labs/conditions@candib80/checks
