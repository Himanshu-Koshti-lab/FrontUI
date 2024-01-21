# HTML CSS Learning

1 to 4 update later

## BOX

# MBPcontent

Margin > --Outline-- > Border > Padding > Content

outline revolve arround border if in +px or inside in -px.

### 09/01 border hack

```css
.box {
  border: 2px solid red;
}
```

to track content properties like padding margin n all.

### 10/01

Card creation done by using
margin auto
padding 10px in icon height,
width 10px line
height 25px
text transform to capital

# To horizontal center by margin auto and given width

# Inline element can't compromise width/height top-bottom margin

### 11/01

Display property working like inline block , inline-block then border-box for maintain size of box,
Display none(save space)
Opacity visibility (not saving space)

Background Shorthand
LG linear gradient
Url for image
P position swap with size left right top bottom
S Size swap with position content cover
R repeat no- repeate space
A Attachment fixed

# Backgroung LG URL PSRA -- shotrcut

    Sample background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(165, 42, 42, 0.384)),
    url("./images/dear.jpg") center/cover no-repeat fixed;

11/01 Background project done

### 12/01

# Relative position

means content will show in diff location from the actual one by using top right bottom left.

# In Absolute

it map to parent relateve content
and you can mark parent content relative by using position relative

### 13/01

Inset shorthand for
top right bottom left while using relative n absolute

### 14/01

# transform

translate
rotate
scale
skew

# transform

to control perticular property to transform and what time it take to transform.

```css
transition-property: transform;
transition-duration: 3s;
```

# animation: name duration timing-function delay iteration-count direction fill-mode;

    Animation shotrcut

# Animation NaDu TiFU DeIt DiFi

    Name custom animation name tag with @Keyframe
    Duration in Sec
    TimingFunction easein/out linear
    Delay in sec
    Iteration 1,2,infinity
    Direction reverse alternate
    Fill-Mode  forward both

Partition transition 0-100 to 0...25..50..100% add multiple transition between keyframe
animation: fromBottom 1s ease-in 0.1s 1 normal forwards;

```css
@keyframes fromBottom {
  0% {
    transform: translateY(10vh);
    opacity: 0;
  }
  100% {
    transform: translateY(0);
    opacity: 1;
  }
}
```

### 15/01

# CSS variable.

```css
--varableName: #ffffff;
```

Font awesome add by link or folder.

# Box Shadow

# Text Shadow

```css
.box {
  width: 200px;
  height: 200px;
  background: rgba(242, 104, 242, 0.67);
  box-shadow: 2px;
  box-shadow: 10px 10px 10px -1px rgba(242, 104, 242, 0.67);
}

/* box-shadow: none | h-offset v-offset blur spread color | inset | initial |
  inherit; */

.text {
  text-shadow: 5px 0px 5px green;
}

/* text-shadow: x-offset y-offset blur-radius color | none | initial | inherit; */
```

#Center Div

````css
.container {
  width: 50%; -- size small
  max-width: 1140px; -- max width
  margin: 0 auto; top/bottom left/right
}```
````

### 16/01

hidden border for rounding image

```css
border: 2px solid rgba(0, 0, 0, 0);
border-radius: 40px;
```

use external-container for controlling size actual size of zoomed image
when hocer to external div internal image got scale

```css
.external-container:hover .inner-image {
  box-shadow: 10px 10px 10px rgb(0, 163, 238);
  transform: scale(1.1);
}
```

### 17/01

Shotcut for creating Div

```css
    (.box.box-${$})*5

    <div class="box box-1">1</div>
    <div class="box box-2">2</div>
    <div class="box box-3">3</div>
    <div class="box box-4">4</div>
    <div class="box box-5">5</div>
```

```css
display: flex; -- Block level border will cover whole width

display:inline-flex -- inline level cover pertivular space which used by child components

```

# Flex-direction

for seting flow of chiled component
row is default
row reverse
column
column-reverse

# Flex-Wrap

to cover screen with if number of elsemt low like text warp in excel.

flex-wrap = wrap/nowrap

# Justify Content

used to Horizontal align child.
space-between space-around

```css
.justify-content-flex-end-container {
  border: 2px solid rgb(0, 255, 21);
  display: flex;
  justify-content: flex-end;
}
.justify-content-center-container {
  border: 2px solid rgb(0, 255, 21);
  display: flex;
  justify-content: center;
}
```

### 18/01

## center

most used

# align item to set child verticaly

```css
.align-item-container {
  height: 400px;
  display: flex;
  flex-direction: row;
  align-items: stretch;
  align-items: center;
}
```

# Align Content to maintain distance between div

```css
.align-content-container {
  height: 100vh;
  display: flex;
  background-color: green;
  flex-direction: row;
  align-items: stretch;
  align-items: center;
  flex-wrap: wrap;
  align-content: center;
  align-content: baseline;
  align-content: end;
  align-content: space-between;
  align-content: space-around;
  align-content: space-evenly;
}
```

### Child level prop for each div\*

# order

set order of div by using order keyword

by default order 0

-1 one for before 1 for after content nondegined order which having default order 0

```css
.align-content-container:hover .box-4 {
  order: -1;
}
```

### 19/01

# flex-grow

it allow you to fill remain space in perticular line or block. by default 0

````css
.align-content-container:hover .box-4 {
  order: -1;
  flex-grow: 1;
}
.align-content-container:hover .box-3 {
  order: -1;
  flex-grow: 3;
}```
````

# Flex shrink

by Default 1
div will shrink if sapve is not there

if set 0
then it will make space for perticular width and move other div to seprate line if space is not there.

```
flex-shrink: 0; be like pushpa jhukega nahi
```

## Flex short cut

Flex: grow shrink width

width set for perticular element

to maintain div in single row trick

````css
.containa {
  display: flex;
  flex-wrap: wrap;
  border: 2px solid red;
}
.boxa {
  flex: 0 1 50%;

}```
````
