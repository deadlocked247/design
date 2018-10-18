# Design guidelines
This is a guide to designing beautiful, delightful experiences at Flip.

Design Tools
- Sketch 
- Adobe After Effects CC 2018
- Adobe Illustrator CC 2018
- Principle

## Interface Design

With interface design we primarily use Sketch. All values are set in px.

### Color

The Flip Blue is what we shade all our colors off of (#1F8EED)

Color must obide the WCAG requirements


> 1.4.3 Contrast (Minimum): The visual presentation of text and images of text has a contrast ratio of at least 4.5:1, except for the following: (Level AA)
> 
> Large Text: Large-scale text and images of large-scale text have a contrast ratio of at least 3:1;
> 
> Incidental: Text or images of text that are part of an inactive user interface component, that are pure decoration, that are not visible to anyone, or that are part of a picture that contains significant other visual content, have no contrast requirement.
> 
> Logotypes: Text that is part of a logo or brand name has no minimum contrast requirement.


### Typography

The fonts we use are Avenir and Tiempos Headline.
The general rule with fonts is if the size is below 20px, use Avenir. If it’s above 20px then use Tiempos Headline.

Avenir: https://www.fontshop.com/families/linotype-avenir
Tiempos: https://klim.co.nz/retail-fonts/tiempos-headline/

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6C18B39D99B66F48970B3F72EF790EFDBB1FBB87EC2D00416425292BA05D2074_1539891246042_Artboard+Copy+3.png)


### Spacing

We use an 8pt grid for spacing elements. Always use multiples of 8 to define dimensions, padding, and margin of both block and inline elements. This is key since most device sizes are divisible by 8. When it comes to spacing, keep in mind the scale factor of the Golden Ratio (1.618).


WCAG guidelines with spacing 


> Line spacing (leading) is at least space-and-a-half within paragraphs, and paragraph spacing is at least 1.5 times larger than the line spacing.



### Vertical Rhythm

Vertical Rhythm is a concept that originated from print typography. In Vertical Rhythm, we try to keep vertical spaces between elements on a page consistent with each other. This means keeping it consistent with a baseline.

Here is an example of using the baseline technique with a base line height of 24px

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6C18B39D99B66F48970B3F72EF790EFDBB1FBB87EC2D00416425292BA05D2074_1539889676621_Artboard+Copy.png)


Implementing Vertical Rhythm from this point on is simple. There are two rules:

- Set the vertical white space between elements to a multiple of 24px.
- Set the line-height of all text elements to a multiple of 24px.

Here the same design with margins, font sizes, and line heights

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6C18B39D99B66F48970B3F72EF790EFDBB1FBB87EC2D00416425292BA05D2074_1539889799517_Artboard.png)


A quick comparison

![](https://d2mxuefqeaa7sj.cloudfront.net/s_6C18B39D99B66F48970B3F72EF790EFDBB1FBB87EC2D00416425292BA05D2074_1539890014264_Artboard+Copy+2.png)




### Quick Tips
- The code is always the final say in design. Prioritize reducing time between ideation and programming over perfect layout in Sketch.


## Artwork and Brand Design

TBD

## References

Google material design https://material.io/design/
Web Content Accessibility Guidelines (WCAG) 2.0 https://www.w3.org/TR/WCAG20/
Making grid systems in Sketch: https://medium.com/sketch-app-sources/8-point-soft-grids-in-sketch-e8f1d5ca2cd4
Why vertical rhythm is important https://zellwk.com/blog/why-vertical-rhythms/

