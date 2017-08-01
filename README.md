# \<polymer-tilt\>

[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/YingshanDeng/polymer-tilt)

Parallax tilt hover effect for Polymer Component, Inspired by [gijsroge/tilt.js](https://github.com/gijsroge/tilt.js), A tiny 60+fps parallax tilt hover effect for jQuery.

![](http://7vikhl.com1.z0.glb.clouddn.com/polymer-tilt.gif)

## Installation
```
bower install --save polymer-tilt
```

## Usage
<!--
```
<custom-element-demo>
  <template>
  <link rel="import" href="polymer-tilt.html">
  <style is="custom-style" include="demo-pages-shared-styles">
    .tilt {
      position: relative;
      display: block;
      width: 100%;
      height: 200px;
      background-color: #08AEEA;
      background-image: linear-gradient(to top, #08AEEA 0%, #2AF598 100%);
      transform-style: preserve-3d;
    }
    .tilt-inner {
      position: absolute;
      top: 50%;
      left: 50%;
      color: white;
      font-size: 20px;
      transform: translateZ(50px) translateY(-50%) translateX(-50%);
    }
  </style>
  <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<polymer-tilt reset>
  <div slot="tilt" class="tilt">
    <div class="tilt-inner">Basic polymer-tilt demo</div>
  </div>
</polymer-tilt>
```

## Options
```js
maxTilt:        10,     // max tilt rotation (degrees)
perspective:    1000,   // Transform perspective, the lower the more extreme the tilt gets
easing:         "cubic-bezier(.03,.98,.52,.99)",    // Easing on enter/exit
scale:          1,      // 2 = 200%, 1.5 = 150%, etc..
speed:          300,    // Speed of the enter/exit transition
axis:           null,   // What axis should be disabled. Can be X or Y
reset:          false,  // If the tilt effect has to be reset on exit
glare:          false,  // Enables glare effect
maxGlare:       1       // From 0 - 1
```

## License
MIT