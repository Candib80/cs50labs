# Fahrenheit

## tl;dr

Implement a program that converts degrees in Celsius to Fahrenheit, per the below, wherein the "0" represents some user's input.

```
$ ./fahrenheit
C: 0
F: 32.0
```

{% next %}

## Turning Up the Heat

In the past, if you wanted to know what the outdoor temperature was, you had to look around for one of these, which might have been mounted outside at your house.

![Image of outdoor thermometer](https://images-na.ssl-images-amazon.com/images/I/71qi9k9byRL._SL1500_.jpg)

Prior to that, if you wanted to know what the temperature was outside, you just stood outside, but we digress. Nowadays, it’s a fairly trivial exercise to pull open a weather app on your phone or visit a weather-reporting website to get the current temperature and the five-day forecast. No need to mess around with one of the above circular dials or its tube-of-mercury cousin.

{% next %}

Depending on where you live in the world, your country uses one of two major temperature scales. If you live in the United States (and don’t spend most of your day working in a science lab), it’s likely that you’re familiar with the Fahrenheit scale, and so if you hear that it’s 30° outside you’re probably putting on a heavy coat and warm pants and bracing yourself for the possibility of snow, because that means it’s quite cold, given that the freezing point of water is 32°. On the other hand, it’s not until the temperature hits 212° that water boils.

In practically every other country of the world (or if you live in the United States and do in fact spend most of your day working in a science lab), you’re probably most familiar with the Celsius or centigrade scale. In that case, if you hear that it’s 30° outside you’re probably going to rummage through your closet for a swimsuit and put on some sunblock, because it’s a beautiful beach day. On the Celsius scale, 0° is the freezing point of water, and 100° is the boiling point.

We acknowledge that with most apps that tell you the weather, it’s fairly simple to press that switch that switches the temperature display from Fahrenheit to Celsius (or vice versa), but before that process was automated for us, one either had to memorize some of the more common conversion points or had to use a mathematical formula to convert from one scale to another, which is important if you plan on traveling internationally.

{% next %}

For this problem, we’re going to focus on converting in just one direction: from Celsius to Fahrenheit. As it happens, the formula for this conversion isn’t terribly complex. (Phew!) One simply takes the current temperature in degrees Celsius (°C), multiplies it by 9, divides by 5, and then adds 32. The result is the equivalent temperature in degrees Fahrenheit (°F). Not bad, right? For the more visually inclined, this translates to this formula:

```
F = ((C * 9) / 5) + 32
```

{% next %}

Let’s do a quick test to make sure things work as expected. Worldwide, the commonly accepted value for normal human body temperature is 37°C. If we plug "37" into that formula where °C goes and do the math (37 multiplied by 9 is 333, 333 divided by 5 is 66.6, 66.6 + 32 is 98.6) we get 98.6°F which is what folks in the United States know as normal human body temperature. So that checks out. Similarly if we plug in 0°C (the freezing point of water) into that formula does it convert to 32°F, and 100°C (the boiling point of water) is apparently equivalent to 212°F. Seems like things are going well.

{% next %}

## Pseudocode

First, write in pseudocode.txt at right some pseudocode that implements this program, even if not (yet!) sure how to writ it in code.

Odds are your pseudocode will use (or imply using!) on or more functions, operators, and variables.

{% spoiler "Hint" %}

There's more than one way to do this, so here's just one!

1. Prompt for degrees Celsius and save this in a variable
2. Use this value to calculate degrees Fahrenheit and save in another variable
3. Print out the result

It's okay to edit your own after seeing this pseudocode here, but don't simply copy/paste ours into your own!

{% endspoiler %}
