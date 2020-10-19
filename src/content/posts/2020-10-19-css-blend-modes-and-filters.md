---
template: blog-post
title: CSS Blend Modes and Filters
slug: /CSS-Blend-Modes-and-Filters
date: 2020-10-18 22:47
description: CSS Blend Modes and Filters
featuredImage: /assets/kelly-sikkema-ereoqdv5s48-unsplash.jpg
---
CSS blend modes and filters allow web developers to design and create many interesting effects. Many of these effects would otherwise require costly and complicated external software such as adobe photoshop. In many cases it is more efficient to create the required effect in CSS, rather than load a larger pre-created image. Another major benefit is that using JS, web designers can animate their CSS blend modes and filters to create interesting dynamic effects on their sites.

So those are some of the surface benefits of CSS blend modes and filters, now to the meat and potatoes: what are the options and how do you use them? Blend is split into two properties; mix-blend-mode, which blends an element with element(or elements) behind it, and background-blend-mode that blends a background image and its background color. These two modes have the following values: color, color-burn, color-dodge, darken, difference, exclusion, hard-light, hue, lighten, luminosity, multiply, normal, overlay, saturation, screen, and soft-light. The CSS filter property has these properties: blur, brightness, contrast, drop-shadow, grayscale, hue-rotate, invert, opacity, saturate, sepia, and url.

Let's start with CSS blend mode:

* **Normal**-The default, the top element will just overlap the elements behind it, it will not change and no blending will occur.
* **Multiply**-The colors of each layer are multiplied together to create the final result. Black always multiplies to black, while white causes no change in color.
* **Screen**-The colors are inverted, multiplied, and then inverted again. This results in the opposite result to multiply. Opposite to multiply, black leads to no change, while white leads to a white layer.
* **Overlay**-This value is **Multiply** on dark areas and **Screen** on light areas. The parts of the top part become lighter where the base is lighter, and darker where the base is darker.
* **Darken**-This one simply uses the darkest value from every layer to create the final result.
* **Lighten**-This value does the opposite of **Darken**, it forms the result using the lightest value of each layer.
* **Color**-Dodge-Similar to **Screen**, this mode divides the bottom layer by the inverted top layer, this results in lightening the bottom layer according to the top layer. As with **Screen**, a white foreground leads to a white result and a black foreground leads to no change.
* **Color-Burn**-This is like **Color-Dodge** for **Multiply** instead of **Screen**. It divides the inverted bottom layer by the top layer, then inverts the result. This darkens the bottom layer according to the top layer. Opposite to **Color-Dodge**, a white foreground changes nothing and a black foreground leads to black.
* **Hard-Light**-This value is like **Overlay**, but with the layers swapped, it acts like **Multiply** where the top is darker, and “**Screen**” where it is lighter.
* **Soft-Light**-The final result is similar to **Hard-Light**, but with a softer, less harsh effect.
* **Difference**-The result is formed by subtracting the darker color from the lighter one. Black has no effect, while white inverts the color.
* **Exclusion**-This value is like **Difference** but with less contrast, resulting in a less harsh effect.
* **Hue**-The result uses the hue of the top layer but the saturation and luminosity of the bottom.
* **Saturation**-The result uses the saturation of the top layer but the hue and luminosity of the bottom.
* **Color**-The result will use the hue and saturation of the top layer, with the luminosity of the bottom.
* **Luminosity**-The result will have the luminosity of the top color, with the hue and saturation of the bottom.

CSS filter has the following functions. Except where noted, they accept a percentage, or a decimal.

* **Grayscale**-This changes the image to grayscale, black and white. 100% is completely grayscale, while 0% is no change.
* **Sepia**-This applies an old photo style sepia filter. 100% is completely sepia, while 0% is unchanged from the original.
* **Saturate**-This function changes saturation of the image. 100% is normal, values over 100% are supersaturated and under 100% are desaturated.
* **Hue-Rotate**-This function “rotates” the hue along the color wheel. This function accepts degrees.
* **Invert**-The original is inverted. 0% is unchanged while 100% in completely inverted.
* **Opacity**-Changes the transparency of the input. 0% is totally transparent, while 100% is unchanged.
* **Brightness**-This alters the brightness of the input. 0% is totally black having no brightness, 100% is unchanged, and values over 100% brighten the image accordingly.
* **Contrast**-Changes the contrast of the input. 0% is completely black, 100% is the original input, and over 100% increases contrast.
* **Blur**-This function applies a gaussian blur to the image. The value is how many pixels on the screen blend together, so a larger value equals more blur. The default value is 0px, percentages are not accepted.
* **Drop**-Shadow-This applies a drop shadow to the input. It is similar to the “box-shadow” CSS property.
* **URL**-This takes a chosen SVG filter and applies to the input.