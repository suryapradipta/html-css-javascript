two main color models:

1. the additive RGB (red, green, blue) model used in electronic devices,
   and
2. the subtractive CMYK (cyan, magenta, yellow, black)
   model used in print.

rgb(red, green, blue);

BLACK background-color: rgb(0, 0, 0); WHITE background-color: rgb(255, 255,
255);

===========================================================================

primary colors:
RED background-color: rgb(255, 0, 0);

GREEN background-color: rgb(0, 255, 0);

BLUE background-color: rgb(0, 0, 255);

===========================================================================

**Secondary colors** are the colors you get when you combine primary
colors. YELLOW background-color: rgb(255, 255, 0);

CYAN background-color: rgb(0, 255, 255);

MAGENTA background-color: rgb(255, 0, 255);

===========================================================================

**Tertiary colors** are created by combining a **primary** with a nearby **
secondary** color.

ORANGE (red, yellow)
background-color: rgb(255, 127, 0);

SPRING GREEN (GREEN, CYAN)
background-color: rgb(0, 255, 127);

VIOLET (MAGENTA, BLUE)
background-color: rgb(127, 0, 255);

There are three more tertiary colors: chartreuse green (green + yellow),
azure (blue + cyan), and rose (red + magenta).

CHARTREUSE GREEN background-color: rgb(127, 255, 0);

AZURE background-color: rgb(0, 127, 255);

ROSE background-color: rgb(255, 0, 127);

A color wheel is a circle where similar colors, or hues, are near each
other, and different ones are further apart. For example, pure red is
between the hues rose and orange.

Two colors that are opposite to each other on the color wheel are called
complementary colors. If two complementary colors are combined, they
produce gray. But when they are placed side-by-side, these colors produce
strong visual contrast and appear brighter.
===========================================================================

Hex color values start with a # character and take six characters from 0-9
and A-F. The first pair of characters represent red, the second pair
represent green, and the third pair represent blue. For example, #4B5320.

GREEN background-color: #00FF00;

You may already be familiar with decimal, or base 10 values, which go from
0 - 9. Hexadecimal, or base 16 values, go from 0 - 9, then A - F:

0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F

===========================================================================

The HSL color model, or hue, saturation, and lightness, is another way to
represent colors.

The CSS hsl function accepts 3 values: a number from 0 to 360 for hue, a
percentage from 0 to 100 for saturation, and a percentage from 0 to 100 for
lightness.

If you imagine a color wheel, the hue red is at 0 degrees, green is at 120
degrees, and blue is at 240 degrees.

Saturation is the intensity of a color from 0%, or gray, to 100% for pure
color. You must add the percent sign % to the saturation and lightness
values.

Lightness is how bright a color appears, from 0%, or complete black, to
100%, complete white, with 50% being neutral.

background-color: hsl(240, 100%, 50%);

===========================================================================

A gradient is when one color transitions into another. The CSS
linear-gradient function lets you control the direction of the transition
along a line, and which colors are used.

One thing to remember is that the linear-gradient function actually creates
an image element, and is usually paired with the background property which
can accept an image as a value.

The linear-gradient function is very flexible -- here is the basic syntax
you'll use in this tutorial:

linear-gradient(gradientDirection, color1, color2, ...); gradientDirection
is the direction of the line used for the transition. color1 and color2 are
color arguments, which are the colors that will be used in the transition
itself. These can be any type of color, including color keywords, hex, rgb,
or hsl.

Now you'll apply a red-to-green gradient along a 90 degree line to the
first marker. background: linear-gradient(90deg, rgb(255, 0, 0), rgb(0,
255, 0)); background: linear-gradient(90deg, rgb(255, 0, 0), rgb(0, 255, 0)
, rgb(0, 0, 255));

===========================================================================

Step 75

You're already familiar with using the rgb function to set colors. To add
an alpha channel to an rgb color, use the rgba function instead.

The rgba function works just like the rgb function, but takes one more
number from 0 to 1.0 for the alpha channel:

rgba(redValue, greenValue, blueValue, alphaValue); You can also use an
alpha channel with hsl and hex colors. You will see how to do that soon.

In the .sleeve rule, use the rgba function to set the background-color
property to pure white with 50% opacity.

===========================================================================


