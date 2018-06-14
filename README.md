[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/monkick/knob-element)

# \<knob-element\>

This is UI like knob or dial.
It select menu with fingers swipe gesture.

## Version
1.0.0

<!--
```html
<custom-element-demo>
  <template>
    <knob-element id="knob" knob-background-image="circle.png" menu-count="9" menu-border="4" smooth="0.99">
      <knob-item class="menu" image="icons/png/001-twitch.png" title="twitch" item-is-selected="true"></knob-item>
      <knob-item class="menu" image="icons/png/002-skype.png" title="skype"></knob-item>
      <knob-item class="menu" image="icons/png/003-snapchat.png" title="snapchat"></knob-item>
      <knob-item class="menu" image="icons/png/004-github.png" title="github"></knob-item>
      <knob-item class="menu" image="icons/png/005-twitter.png" title="twitter"></knob-item>
      <knob-item class="menu" image="icons/png/006-facebook.png" title="facebook"></knob-item>
      <knob-item class="menu" image="icons/png/003-snapchat.png" title="snapchat"></knob-item>
      <knob-item class="menu" image="icons/png/004-github.png" title="github"></knob-item>
      <knob-item class="menu" image="icons/png/003-snapchat.png" title="snapchat"></knob-item>
      <knob-item class="menu" image="icons/png/004-github.png" title="github"></knob-item>
      <knob-item class="menu" image="icons/png/003-snapchat.png" title="snapchat"></knob-item>
      <knob-item class="menu" image="icons/png/004-github.png" title="github"></knob-item>
    </knob-element>
  </template>
</custom-element-demo>
```
-->

## Installation

```
$ bower install --save monkick/knob-element
```

## Usage

At first. Import it at header.

```html
    <link rel="import" href="../bower_components/knob-element/knob-element.html">
    <link rel="import" href="../bower_components/knob-element/knob-item.html">
```

Next. Add the `knob-element` custom tag and put some `knob-item` in `knob-element`.

```
    <knob-element id="knob" knob-background-image="circle.png" menu-count="9" menu-border="4" smooth="0.99">
      <knob-item class="menu" image="icons/png/001-twitch.png" title="twitch" item-is-selected="true"></knob-item>
      <knob-item class="menu" image="icons/png/002-skype.png" title="skype"></knob-item>
      <knob-item class="menu" image="icons/png/003-snapchat.png" title="snapchat"></knob-item>
      <knob-item class="menu" image="icons/png/004-github.png" title="github"></knob-item>
      <knob-item class="menu" image="icons/png/005-twitter.png" title="twitter"></knob-item>
      <knob-item class="menu" image="icons/png/006-facebook.png" title="facebook"></knob-item>
      <knob-item class="menu" image="icons/png/003-snapchat.png" title="snapchat"></knob-item>
      <knob-item class="menu" image="icons/png/004-github.png" title="github"></knob-item>
      <knob-item class="menu" image="icons/png/003-snapchat.png" title="snapchat"></knob-item>
      <knob-item class="menu" image="icons/png/004-github.png" title="github"></knob-item>
      <knob-item class="menu" image="icons/png/003-snapchat.png" title="snapchat"></knob-item>
      <knob-item class="menu" image="icons/png/004-github.png" title="github"></knob-item>
    </knob-element>
```

Able to use `dom-repeat`

```
    <knob-element id="repeat" knob-background-image="circle.png" menu-count="9" menu-border="4" knob-speed="550">
      <dom-repeat id="drepeat" initial-count="4" items="[[items]]">
        <template>
          <knob-item class="menu" image="[[item.image]]" title="[[item.title]]"></knob-item>
        </template>
      </dom-repeat>
    </knob-element>
```

## Parameter

### knob-element

| key | default | description |
|----------------|-------------|-------------| 
| degree | 0 | degree of menu now |
| selected | - | Item No of selected now |
| distance | 125 | Distance of menu from base point |
| knob-background-image | '' | URL of background image path |
| menu-count | 6 | count of menu |
| menu-border | 3 | Border of visible or disappear for menu |
| menu-start-position | 90 | Start position of menu. This value is degree unit |
| knob-width | - | Width of knob |
| knob-height | - | Height of knob |
| disable-event | false | disable gesture |
| smooth | 0.65 | Number of smooth of knob animation |
| knob-speed | 0 | knob's transition time |
| knob-action | end | user's gesture (start, track, end) |

### knob-item

| key | default | description |
|----------------|-------------|-------------|
| image | - | knob background image |
| itemWidth | 40px | width of item |
| itemHeight | 40px | height of item |
| title | - | title of menu |
| itemTop | - | location of item from top |
| itemLeft | - | location of item from left |
| itemDisplay | - | display property of css |
| itemWillChange | inherit | willchnage property of css |
| itemTransform | - | transform property of css |
| itemIsSelected | - | selected |
| icon | - | iron-icons name |


## Event

| key | param | description |
|----------------|-------------|-------------|
| menu-click | selected | fire event when menu clicked |
| changed | selected | fire event when menu chnaged |