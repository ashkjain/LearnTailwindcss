# LearnTailwindcss

# Colors:
## Text Colors:
The class that we use for text color is simply called `text` and then we add the name of the color with adding hypen and the name of the color, like this: `text-black`. But to be noticed black and white does not have a shade but other colors come in shades starting from 50 - 900. There are various colors provided by css, please refer to tailwindcss docs.
## Background Colors:
As same as the text we also have classes for background color, the class that we use is called `bg` and then name of the color and the shade seprated by the hypen, for example `bg-red-500`. The best thing about tailwindcss that we can refer to or combine multiple classes. For example black background and black text does not make sense so we can do something like this: 
```
<p class="bg-black text-white>Some Text</p>
```
Just remember to seperate the classes with whitespace.
## Text Underline:
To give a text an underline we just simply have to say underline in class. But it will just give you a black underline, to add some color we can use the class called decoration. Here is the example to apply it: -
```
<p class="underline decoration-red-500>Some text</p>
```
## Border Color
To apply a border color you just simply have to declare the class `border-nameofcolor-(50-900)`. Let me show it in this example, but make sure there is a border already applied to color it, if there is no border the color won't apply. Here is the example:
```
<input type="text" class="border border-green-800">
```

## Divide Colors
First we have to divide something in sets or like a list then we apply the class called `divide-(y or x)`, and since the main div has the divide property we can change color. Here is the example:
```
<div class="divide-y divide-blue-300">
<div>Item 1</div>
<div>Item 2</div>
</div>
```
Now there is a division between item 1 and 2, and the division or the line that divide them has a color of blue with shade 300

## Outline colors:
Same goes for outline we can declare the class to create an outline and then declare another class outline and the color. Here is the example:
```
<button class="outline outline-blue-300">Submit Me</button>
```

## Box Shadow COlors, default value set to 100
We can also create box shadow on an element, first make sure to declare type of shadow (lg, md, sm) then the color of it with depth. Here is the example:
```
<button class="shadow-lg bg-cyan-500 shadow-purple-500/60">Subscribe</button>
```
And the slash and the number means the opacity which is set to 100.

## Accent Colors
We can use accent color and we just need to type accent and then the color name and the shade of the color. Here is the example:
```
<input type="checkbox" class="accent-purple-500">
```

## Arbitrary Colors
We can also add arbitrary color or several colors, and it could be RGB, color names, or the hex value. To do that we have to specify what type like bg, shadow, text, and them hyphen and square brackets contains that color code. Here is the example:
```
<div class="bg-[cyan]">Hello</div>
```

# Container and Spacing
## Container
To declare a container we have to specify a class called `container` which has various breakpoints.

## Margin
THere are also some margin pre-defined classes, first and foremost `mx-auto` and `my-auto` can put margin auto based on the axis. X: Left and Right, and Y: Top and Bottom. To define the margin on all side we use `m-{number}`, so lets say we want 8px margin on every side we will do something like this: `m-2`. If we want margin on right, left, bottom, or top, we will just add the first letter of the side with 'm'. Lets see an example for margin right 4px: `mr-1`. So the unit 1 = 0.25 rem or 4px. And when then increase it increase in the multplication. So 4 would be 1rem or 16px. The limit of these number are 0.5 to 96. We can also provide it an arbitrary value in square brackets something like number of pixels.

## Padding
Padding is same as Margin values, instead of `m` it will just be `p`. So padding right 1rem or 16px would be `pr-4`.

## Space Between X
So space between the x-axis is used something like flexbox or the navbar, to seperate the content on the x-axis we use space between x. To apply this we simply say, for example space between x 1rem : `space-x-4`.

## Space Between Y
Same goes for Space between Y as space between x, just the x is swapped with Y. So it would look something like this: `space-y-4`.

# Typography:
## Font Family:
There are basically three main font family that we can use using tailwindcss but we can also create our custom configuration for those. Lets see default first, these three are default:
```
<div class="font-sans">Tailwind is Awesome</div>
<div class="font-serif">Tailwind is Awesome</div>
<div class="font-mono">Tailwind is Awesome</div>
```
To config new fonts we can use script tag and pass this:
```
<script>
        tailwind.config = {
            theme:{
                fontfamily: {
                    'sans': ['ui-sans-serif','system-ui'],
                    'serif': ['ui-serif','Georgia'],
                    'mono': ['ui-monospace','SFMono-Regular'],
                }
            }
        }
    </script>
```
And we can bring more fonts using link and change the first content of the array with the new font we want for sans, serif, or mono.

## Font Size:
To add the font size or add the fond size there is a class called text and then the size. There are a list of sizes that can be used. Here is the list: xs, sm, base, lg, xl, 2-9xl. These are in the order. This is how to apply them:
```
<p class="text-lg">This is text</p>
```

## Font Weight:
To apply font weight we just have to simply use font hyphen and type of weight, these are the types: light, normal, medium, semibold, bold. This is how we can apply:
```
<p class="font-semibold">This is some text</p>
```

## Letter Spacing
There are only three classes for letter spacing, to apply we have to use class called tracking-(type of spacing), the types are, tight, normal, and wide. Here is how you apply it:-
```
<p class="tracking-wide">Some random text</p>
```

## Text Alignment:
We have basically three classes to set the alignment, left, center, and right, to apply this we have to preceed with text then hyphgen and the type. Here is how to apply this:
```
<p class="text-left">Some random value</p>
<p class="text-center">Some random value</p>
<p class="text-right">Some random value</p>
```

## Text Decoration, style, and offset
To set the decoration there are 4 decorations, underline, overline, line-through, and no-underline. And adding a style on these decoration, we use decoration class with type of decoration like name of the color and the shade, or if we want to make decoration look differenet there are 5 more styles: solid, double, dotted, dashed, and wavy. We can also give the decoration thickness, with number ranging from 0-8. We can also change the offset of the undeline by using the underline-offset class and adding the number ranging from 0-8. Here are the examples of all of them:-
```
<div class="underline decoration-4 decoration-blue-400">Some Text</div>
    <div class="underline decoration-dotted">Some Text</div>
    <div class="underline decoration-double">Some Text</div>
    <div class="underline decoration-dashed">Some Text</div>
    <div class="underline decoration-4 decoration-blue-400 underline-offset-4">Some Text</div>
```

## Text transforr:
In this we have four class or properties, uppercase, lowercase, normal-case, and capitalize to change the text occurence. Here is the example:
```
  <p class="uppercase">This is all uppercase</p>    
    <p class="normal-case">This is all normal</p>
    <p class="lowercase">This is all LOWECASE</p>
    <p class="capitalize">this is all capitalize</p>
```