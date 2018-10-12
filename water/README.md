# Water

## tl;dr

Implement a program that reports a user’s water usage, converting minutes spent in the shower to bottles of drinking water, wherein the "1" and "10" are input from the user.

```
$ ./water
Minutes: 1
Bottles: 12

$ ./water
Minutes: 10
Bottles: 120

```

{% next %}

## Background

Suffice it to say that the longer you shower, the more water you use. But just how much? Even if you have a "low-flow" showerhead, odds are your shower spits out 1.5 gallons of water per minute. A gallon, meanwhile, is 128 ounces, and so that shower spits out 1.5 × 128 = 192 ounces of water per minute. A typical bottle of water (that you might have for a drink, not a shower), meanwhile, might be 16 ounces. So taking a 1-minute shower is akin to using 192 ÷ 16 = 12 bottles of water. Taking (more realistically, perhaps!) a 10-minute shower, then, is like using 120 bottles of water. Deer Park, that’s a lot of water! Of course, bottled water itself is wasteful; best to use reusable containers when you can. But it does put into perspective what’s being spent in a shower!

{% next %}

## Specification

- To the right you will see `water.c` where you will create a program that prompts the user for the length of his or her shower in minutes (as a positive integer) and then prints the equivalent number of bottles of water (as an integer)

- You will comment your name at the very top, where indicated to do so

- For simplicity, you may assume that the user will input a positive integer, so no need for error-checking (or any loops) this time! And no need to worry about overflow!

{% next %}

## Walkthrough

{% video https://www.youtube.com/watch?v=oAcVHgmjTHE&feature=youtu.be %}

{% spoiler "Hint" %}

- You can use the function `get_int` to prompt the user to input an integer value, as per below:

```
int minutes = get_int("put your prompt here");
```

{% endspoiler %}

{% next "Checks" %}

## Check Your Work

Be sure to `make` your program via the following:

```
make water
```

Then run your program via:

```
./water
```

Entering a valid amount of minutes of your shower, including, but not limited to, the ones given at the top of the lab.

---

To check your work via check50, run the following in the terminal window

```
check50 cs50/2017/x/water
```

{% next "Submit" %}

## Submit

Execute the below, logging in with your GitHub username and password when prompted. For security, you'll see asterisks (`*`) instead of the actual characters in your password.

```
submit50 cs50/2017/x/water
```
