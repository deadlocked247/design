# Flip design guidelines
This is a guide to designing beautiful, delightful experiences at Flip.

## Table of Contents
Interface Design

1. [Color](#color)
2. [Typography](#typography)
3. [Spacing](#spacing)

Design Tools

* Sketch 
* Adobe After Effects CC 2018
* Adobe Illustrator CC 2018
* Principle

## Interface Design

With interface design we primarily use Sketch. All values are set in px.

### <a name="color"></a> Color

The Flip Blue is what we shade all our colors off of (#1F8EED)

Color must obide the WCAG requirements


> 1.4.3 Contrast (Minimum): The visual presentation of text and images of text has a contrast ratio of at least 4.5:1, except for the following: (Level AA)
> 
> Large Text: Large-scale text and images of large-scale text have a contrast ratio of at least 3:1;
> 
> Incidental: Text or images of text that are part of an inactive user interface component, that are pure decoration, that are not visible to anyone, or that are part of a picture that contains significant other visual content, have no contrast requirement.
> 
> Logotypes: Text that is part of a logo or brand name has no minimum contrast requirement.


### <a name="typography"></a>Typography

The fonts we use are Avenir and Tiempos Headline.
The general rule with Tiempos Headline is to use it for titles and larger font sizes. 

Avenir: https://www.fontshop.com/families/linotype-avenir
Tiempos: https://klim.co.nz/retail-fonts/tiempos-headline/

**Print design typography**

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6C18B39D99B66F48970B3F72EF790EFDBB1FBB87EC2D00416425292BA05D2074_1539891246042_Artboard+Copy+3.png)


**Web design typography**

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6C18B39D99B66F48970B3F72EF790EFDBB1FBB87EC2D00416425292BA05D2074_1539893057431_Artboard+Copy+5.png)


WCAG guidelines with line-height 

> Line spacing (leading) is at least space-and-a-half within paragraphs, and paragraph spacing is at least 1.5 times larger than the line spacing.


### <a name="spacing"></a>Spacing

We use an 8pt grid for spacing elements. Always use multiples of 8 to define dimensions, padding, and margin of both block and inline elements. This is key since most device sizes are divisible by 8. When it comes to spacing, keep in mind the scale factor of the Golden Ratio (1.618). The spacing between elements is via relative positioning.

**Why a relative spacing vs absolute spacing?**

When it comes time to code up an interface, using an actual grid is irrelevant because programming languages don’t use that kind of grid structure - it’ll just get thrown away. Using a more fluid, minimal structure can be an advantage when it comes time to code your design.


We use the **box model** at Flip. The box model is a way to describe an object’s dimensions and spacing.

* **Border**: the thickness of the stroke around the edges of an element.

* **Padding**: the space between the bounds of an element and its child elements

* **Margin**: the space between the bounds of an element and neighboring objects


![](https://d2mxuefqeaa7sj.cloudfront.net/s_6C18B39D99B66F48970B3F72EF790EFDBB1FBB87EC2D00416425292BA05D2074_1539892450171_Artboard+Copy+4.png)


#### Vertical Rhythm

Vertical Rhythm is a concept that originated from print typography. In Vertical Rhythm, we try to keep vertical spaces between elements on a page consistent with each other. This means keeping it consistent with a baseline.

A quick comparison

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6C18B39D99B66F48970B3F72EF790EFDBB1FBB87EC2D00416425292BA05D2074_1539890014264_Artboard+Copy+2.png)


Here is an example of using the baseline technique with a base line height of 16px

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6C18B39D99B66F48970B3F72EF790EFDBB1FBB87EC2D00416425292BA05D2074_1539889676621_Artboard+Copy.png)


#### Example of vertical rhythm

Baseline value: **16px**

Line-height scale: **1.5**

Scale factor: **1.618** (golden ratio)

Margin size: baseline * 2 = **24px**


Line-heights via line-height scale
> 16 * (1.5 * 0) = **16px**
> 
> 16 * (1.5 * 1) = **24px**
>
> 16 * (1.5 * 2) = **48px**
> 
> 16 * (1.5 * 3) = **72px**

Font-sizes via scale factor (rounded values)
> 16 * (1.618 ^ 1) = **25.88 = ~26px**
>
> 16 * (1.618 ^ 2) = **41.86 = ~42px**
> 
> 16 * (1.618 ^ 3) = **67.772 = ~68px**

Rule to combine line height to a font size:
Find the minimum line height where `lineHeight > fontSize`

```
h1 {
	font-size: 68px;
	line-height: 72px;
}

h2 {
	font-size: 42px;
	line-height: 48px;
}
...
```

Here the same design with margins, font sizes, and line heights

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6C18B39D99B66F48970B3F72EF790EFDBB1FBB87EC2D00416425292BA05D2074_1539894971131_Artboard.png)

#### Formulas to calculate sizes and scale
Here are simple formulas you can use to find:

1) The adjusted line height, given a font size and line width

![](https://pearsonified.com/wp-content/uploads/2011/12/line-height-ratio.gif)

2) The adjusted line width, given a font size and line height 

![](https://pearsonified.com/wp-content/uploads/2011/12/line-width.gif)

#### Examples

> I want to use a 16px font size in a content width of 550px

We can use 1) here to find the line height.


![](https://pearsonified.com/wp-content/uploads/2011/12/line-height-ratio-16-550.gif)

1.56216 is our **line-height scale**. We can use this to find the final line-height value by multiplying it with the baseline value.


![](https://pearsonified.com/wp-content/uploads/2011/12/line-height-16-550.gif)

Our final line-height value is 125.00169 = **~25px**

> I want to use a 16px font size with a line-height of 26px

We can use 2) here to find the width

![](https://pearsonified.com/wp-content/uploads/2011/12/line-width-16-26.gif)

Width = 685.32505 = **~685px**



### Quick Tips
- The code is always the final say in design. Prioritize reducing time between ideation and programming over perfect layout in Sketch.


## Artwork and Brand Design

TBD

### References

* Google material design https://material.io/design/
* Web Content Accessibility Guidelines (WCAG) 2.0 https://www.w3.org/TR/WCAG20/
* Making grid systems in Sketch: https://medium.com/sketch-app-sources/8-point-soft-grids-in-sketch-e8f1d5ca2cd4
* Why vertical rhythm is important https://zellwk.com/blog/why-vertical-rhythms/

