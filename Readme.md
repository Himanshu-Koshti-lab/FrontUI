# HTML CSS Learning

1 to 4 update later

## BOX

MBPcontent

Margin > --Outline-- > Border > Padding > Content

outline revolve arround border if in +px or inside in -px.

09/01 border hack

```css
.box {
  border: 2px solid red;
}
```

to track content properties like padding margin n all.

### 10/01

Card creation done by using margin auto padding 10px in icon height and width10px line height 25px text transform to capital

To horizontal center by margin auto and given width

Inline element can't compromise width/height top-bottom margin

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

    Backgroung LG URL PSRA  -- shotrcut

    Sample background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(165, 42, 42, 0.384)),
    url("./images/dear.jpg") center/cover no-repeat fixed;

11/01 Background project done

### 12/01

Relative positionmeans content will whow in diff location from the actual one by using top rightbottom left.

In Absolute it map to parent relateve content
and you can mark parent content relative by using position relative

### 13/01

Inset shorthad for
top right bottom left while using relative n absolute

### 14/01

transform
translate
rotate
scale
skew

to control perticular property to transform and what time it take to transform.

```css
transition-property: transform;
transition-duration: 3s;
```

animation: name duration timing-function delay iteration-count direction fill-mode;

    Animation shotrcut
    Animation NaDu TiFU DeIt DiFi

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
