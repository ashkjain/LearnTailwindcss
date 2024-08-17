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