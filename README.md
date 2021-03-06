# ScrollUp 2.1.0 [![Build Status](https://travis-ci.org/markgoodyear/scrollup.png?branch=master)](https://travis-ci.org/markgoodyear/scrollup)

## Installing with Bower
To install scrollUp with Bower:

```
bower install scrollup
```

## How to use
Simply include the `jquery.scrollUp.min.js` file and place the following in the head of your document (make sure jQuery is included):

### Minimum setup

```
$(function () {
    $.scrollUp();
});
```

**Example with default options**

```
$(function () {
    $.scrollUp({
        scrollName: 'scrollUp', // Element ID
        scrollDistance: 300, // Distance from top/bottom before showing element (px)
        scrollFrom: 'top', // 'top' or 'bottom'
        scrollSpeed: 300, // Speed back to top (ms)
        easingType: 'linear', // Scroll to top easing (see http://easings.net/)
        animation: 'fade', // Fade, slide, none
        animationInSpeed: 200, // Animation in speed (ms)
        animationOutSpeed: 200, // Animation out speed (ms)
        scrollText: 'Scroll to top', // Text for element, can contain HTML
        scrollTitle: false, // Set a custom <a> title if required. Defaults to scrollText
        scrollImg: false, // Set true to use image
        activeOverlay: false, // Set CSS color to display scrollUp active point, e.g '#00FFFF'
        zIndex: 2147483647 // Z-Index for the overlay
    });
});
```

### activeOverlay

To create a visible line to help determine an ideal scroll distance from the top, assign a valid CSS colour to the `activeOverlay` setting. This could be HEX, HSLA or RGB(A). Example: `activeOverlay: '#00FFFF'`. <a href="http://markgoodyear.com/labs/scrollup" target="_blank">See the demo for an example</a>.
<p style="text-align: center;"></p>

### scrollFrom

New feautre in v2.0.0. Display the scrollUp element either the set distance from the top (default), or from the bottom of the page.

### Destroy method

New feautre in v2.0.0. If you need to destroy the instance of scrollUp, simple use the following to remove all modifications to the DOM:

```
$.scrollUp.destroy();
```


## Fully Customizable
ScrollUp is fully customizable via CSS which makes it simple to fit right into your project. Simply target the scrollUp's generated ID in your CSS file and set your styles. Below is a basic style example:

```
#scrollUp {
    bottom: 20px;
    right: 20px;
    padding: 10px 20px;
    background: #555;
    color: #fff;
}
```

### Use background image

To use a background image instead of text, simply set `scrollImg: true`. This will allow you to set a background image in your CSS file.

## Contributing
Please see [CONTRIBUTE.md](CONTRIBUTE.md) for info on contributing.

## Demo
<a href="http://markgoodyear.com/labs/scrollup/" target="_blank">Check out the demo</a> for more style and feature examples.


start a improve
