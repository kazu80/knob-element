# \<knob-element\>

ui of like knob

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

## Parameter

| key | default | description |
|----------------|-------------|-------------| 
| distance | 125 | Distance of menu from base point |
| menu-border | 3 | Border of visible or disappear for menu |
| menu-start-position | 90 | Start position of menu. This value is degree unit |  

