# proxima

### Proxima is a SCSS library that will let you cyberpunkify your site.

### Ways to use:
You can download it [**here**](https://github.com/pixelgalaxies/proxima/raw/master/proxima.zip).

Then in your SCSS/SASS file you can do:
@use 'proxima' as *;

or

import '/pathto/proxima.scss'

### Lines

#### Classes
##### .p-underline-1
##### .p-underline-2
##### .p-underline-3
##### .p-underline-4
##### .p-underline-5
#### Glitch Classes
##### .p-flip
##### .p-bungle-1
##### .p-bungle-2
##### .p-bungle-3
##### .p-bungle-4
##### .p-bungle-5
#### Mixins
##### @include underline($line-color, $line-height);

> These classes can go on any element and will use the after pseudo element to create an underline accent. The mixin takes in the color of the line and the line height, defaults are black and 2.

```
<span class="p-underline-1 p-flip">.p-underline-1.p-flip</span>
<span class="p-underline-1 p-bungle-1">.p-underline-1.p-bungle-1</span>
<span class="p-underline-2 p-bungle-2">.p-underline-2.p-bungle-2</span>
<span class="p-underline-3 p-bungle-3">.p-underline-3.p-bungle-3</span>
<span class="p-underline-4 p-bungle-4">.p-underline-4.p-bungle-4</span>
<span class="p-underline-5 p-bungle-5">.p-underline-5.p-bungle-5</span>
```




### Buttons

#### Classes
##### .p-btn-1
##### .p-btn-2
##### .p-btn-3
#### Glitch Classes
##### .p-btn-glitch
##### .p-btn-hover-glitch

#### Mixins
##### @include button-bg($bg-color, $bg-color-hover); 

> These classes use the before pseudo element for their glitch effect. The mixin takes in the color of the line and the line height. 

```
<button class="p-btn-1">.p-btn-1</button>
<button class="p-btn-2">.p-btn-2</button>
<button class="p-btn-3">.p-btn-3</button>

<button class="p-btn-2 p-btn-glitch">.p-btn-glitch</button>
<button class="p-btn-2 p-btn-hover-glitch">.p-btn-hover-glitch</button>
```




### Boxes

#### Classes
##### .p-boxes-1
##### .p-boxes-2
##### .p-boxes-3
##### .p-boxes-4
##### .p-boxes-5


> The box classes give any your elements a cyberpunk-esque border. Don't forget to set you border color when using these classes.

```
<div class="p-box-1">
	<span>.p-box-1</span>
</div>
<div class="p-box-2">
	<span>.p-box-2</span>
</div>
<div class="p-box-3">
	<span>.p-box-3</span>
</div>
<div class="p-box-4">
	<span>.p-box-4</span>
</div>
<div class="p-box-5">
	<span>.p-box-5</span>
</div>
```





### Cutouts

#### Classes
##### .p-cutout-1
##### .p-cutout-2
##### .p-cutout-3
##### .p-cutout-4
##### .p-cutout-5


> Cutouts are a set of classes that are basically the reverse of the boxes. Instead of an outline, the element will have a background fill. Don't forget to set a background color when using these classes.

```
<p class="p-cutout-1">
	.p-cutout-1
</p>
<p class="p-cutout-2">
	.p-cutout-2
</p>
<p class="p-cutout-3">
	.p-cutout-3
</p>
<p class="p-cutout-4">
	.p-cutout-4
</p>
<p class="p-cutout-5">
	.p-cutout-5
</p>
```




### Hypertext

#### Class
##### .p-hypertext

#### Mixin
##### @include hypertext($color-1, $color-2, $color-3);



> The Hyper Text class applies a tri-color overlay to an element. It uses a data attribute called "data-hypertext" which should have the same value as the innerHTML and uses pseudo elements to create the glitching effect.

```
<span class="p-hypertext" data-hypertext=".p-hypertext">
	.p-hypertext
</span>

```





### Cursors

#### Classes
##### .p-cursor-underline
##### .p-cursor-line
##### .p-cursor-block



> These classes will use the after pseudo-element and create a blinking cursor after some text.

```
<span class="p-cursor-underline">.p-cursor-underline</span>
<span class="p-cursor-line">.p-cursor-line</span>
<span class="p-cursor-block">.p-cursor-block</span>

```





### Trims

#### Classes
##### .p-trim-1
##### .p-trim-2
##### .p-trim-3
##### .p-trim-bottom

#### Mixin
##### @include trim($bg-color, $before-color, $after-color, $text-color);



> These are the most complicated classes to use of the library. It's recommended to give the trim elements another class (i.e. p-odd) then pass them all the corresponding mixin. Then the "other" non-trim elements can get a class like p-even to be styled all at once. The last element will need the p-trim-bottom class and will accept the trim mixin.

```
<div class="p-trim-1 p-odd"></div>
<div class="p-even"></div>
<div class="p-trim-2 p-odd"></div>
<div class="p-even"></div>
<div class="p-trim-3 p-odd"></div>
<div class="p-trim-bottom p-even"></div>

```





### General Glitches

#### Classes
##### .p-glitch
##### .p-glitch-hover
##### .p-glitch-fast
##### .p-glitch-faster
##### .p-glitch-slow
##### .p-glitch-slower


> These are the just general glitches. Throw them on any element and the element will spazz out. 

```
<p class="p-glitch">.p-glitch</p>
<p class="p-glitch-hover">.p-glitch-hover</p>

<p class="p-glitch-fast">.p-glitch-fast</p>
<p class="p-glitch-faster">.p-glitch-faster</p>

<p class="p-glitch-slow">.p-glitch-slow</p>
<p class="p-glitch-slower">.p-glitch-slower</p>

```





### Background Textures

#### Classes
##### .p-dotted
##### .p-crossed
##### .p-connected

#### Mixins
##### @include dotted($dot-color, $size);
##### @include crossed($cross-color, $size);
##### @include connected($line-color, $dot-color);



> There are three mixins for the goodies section, each pertaining to their respective background textures. Note: You MUST use an RGBA value for these three mixins.

```
<div class=p-dotted"></div>

<div class="p-crossed"></div>

<div class="p-connected"></div>


```




