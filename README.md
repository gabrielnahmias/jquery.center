# jQuery Center Plugin

A jQuery plugin that centralizes DOM elements.

## Description

This simple plugin helps you centralize any DOM element against its parent element or window. You can also specify the top of the DOM element by passing customized settings. This plugin only works for **absolute elements**.

## Demo
 - Please see `demo.html`.
 - For a live demo, please take a look at [this](http://dreamerslab.com/demos/centralize-html-dom-element-with-jquery-center-plugin).

## Documentation
  - For the Chinese version, please go [here](http://dreamerslab.com/blog/tw/centralize-html-dom-element-with-jquery-center-plugin/).

## Requires
  - jQuery 1.2.6+

## Browser Compatibility
  - [Firefox](http://mzl.la/RNaI) 2.0+
  - [Internet Explorer](http://bit.ly/9fMgIQ) 6+
  - [Safari](http://bit.ly/gMhzVR) 3+
  - [Opera](http://bit.ly/fWJzaC) 10.6+
  - [Chrome](http://bit.ly/ePHvYZ) 8+

## Installation
  - First, make sure you are using a valid [DOCTYPE](http://bit.ly/hQK1Rk).
  - Include the necessary JS files (jQuery, etc.).

```html
<script type="text/javascript" src="http://code.jquery.com/jquery-latest.min.js"></script>
<script type="text/javascript" src="jquery.center.js"></script>
```

## Options

#### against
  - **Description:** the element against which the DOM element centralizes
  - **Data Type:** string
  - **Default Value:** `"window"`
  - **Possible Value:** `"window"`, `"parent"`, or `".someTarget"`

#### top
  - **Description:** you can specify the top of the target element in pixels...
  - **Data Type:** integer
  - **Default Value:** `false`
  - **Possible Value:** `13`, `20`, `36`... any number you want

#### topPercentage
  - **Description:** ... or specify the top in percentage of the target element
  - **Data Type:** float
  - **Default Value:** `0.5`
  - **Possible Value:** `0.1`, `0.4`, `0.8`...

#### resize
  - **Description:** center on window resize?
  - **Data Type:** boolean
  - **Default Value:** `true`
  - **Possible Value:** `true` or `false`

## Usage
> Example code:

```javascript
// centralize #some-element against the window
$('#some-element').center();

// centralize .some-element against its parent element
$('.some-element').center({
	against : 'parent',
	top     : 10
});

// centralize .some-element against '.some-target-element'
// !IMPORTANT '.some-target-element' must be ".some-element"'s parents
$('.some-element').center({
	against       : '.some-target-element',
	topPercentage : 0.4
});
```

## License

The expandable plugin is released under the MIT License (`LICENSE.txt`).

Copyright (c) 2011 [Ben Lin](http://dreamerslab.com) with modifications by [Gabriel Nahmias](http://terrasoftlabs.com).