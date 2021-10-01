# automated-a11y-sass
Sass functions that support accessible color contrast ratios

## Requirements

Minimum Sass version 3.4.25. Libsass 3.5.4 (best performance).

## Sandboxes

[Editable sandbox on CodePen to see how this all works](https://codepen.io/jhogue/pen/jOEXxZe?editors=0100). Change the color variables to see the updates in real-time within the size tests. 

When an edge case has been encountered, a version in SassMeister with debug output is helpful to see what might be happening (I changed the main function to a mixin so I can debug the output): 

[sassmeister.com/gist/42b8402a3cb5ac41f8557df4e175b1f7](https://www.sassmeister.com/gist/42b8402a3cb5ac41f8557df4e175b1f7)

## Article with Full Explanation

[Programming Sass to Create Accessible Color Combinations](https://css-tricks.com/programming-sass-to-create-accessible-color-combinations/)


## Acknowledgments

+ Previous ideas used lots of math to replicate a `pow()` function but it was not performant. Then I used a lookup table and that worked pretty well. Better still, [Merovex](https://github.com/Merovex) provided a succinct and performant `pow()` from [Hail2u](https://gist.github.com/hail2u/1964056)
+ Luminance function adapted from [Sérgio Gomes](https://medium.com/dev-channel/using-sass-to-automatically-pick-text-colors-4ba7645d2796) who borrowed code from [voxpelli](https://gist.github.com/voxpelli/6304812)
+ “Light or Dark?” function also adapted from Sérgio Gomes
+ Contrast ratio calculation adapted from Lea Verou’s [Color.js](https://github.com/LeaVerou/contrast-ratio/blob/gh-pages/color.js)
+ Debugging the `@while` Sass statement help from [Merovex](https://github.com/Merovex)
+ And finally, lots of other various sources of math and approaches to this until I came across the best way to do things (so far)
