# Custom checkboxes

A light and simple way to custom your form checkboxes.

## How it works

This library hides the checkboxes designated as to be customized, and creates graphic clones from `<div>` tags.
Checked state is synchronized between them.

## Project status

This version is the 1.0.0 stable version, this should work smoothly on most browsers.

## Installation

1. Copy this project in your vendor/ directory
2. Link the `styles.min.css` CSS between the `<head>` and closing `</head>`tags
``` html
  <head>
    <link rel="stylesheet" media="screen" href="vendor/custom-checkboxes-master/themes/styles.min.css" type="text/css">
  </head>
```
3. Call the custom checkboxes library before the closing `</body>` tag and call immediately after the `custCbx()` function:
``` html
  <script type="text/javascript" src="vendor/custom-checkboxes-master/js/customCheckboxes_1.0.min.js"></script>
  <script>
    custCbx();
  </script>
</body>
```

## Usage

Add the `custCbx` class to all checkboxes to customize.

***Notice:*** All checkboxes must have an id.

***Notice:*** Checkboxes can be prechecked.

You can add styling classes:

### Manage shape (default: square)
* ![custCbx-square](/example/custCbx-square.png?raw=true) custCbx-square
* ![custCbx-rounded](/example/custCbx-rounded.png?raw=true) custCbx-rounded
* ![custCbx-round](/example/custCbx-round.png?raw=true) custCbx-round
* ![custCbx-tick](/example/custCbx-tick.png?raw=true) custCbx-tick
* ![custCbx-tick](/example/custCbx-cross.png?raw=true) custCbx-cross

### Manage animation (default: no animation)
* ![custCbx-fading](/example/custCbx-fading.gif?raw=true) custCbx-fading
* ![custCbx-checking](/example/custCbx-checking.gif?raw=true) custCbx-checking
* ![custCbx-checking](/example/custCbx-crossing-out.gif?raw=true) custCbx-crossing-out

### Manage color (default: black)
* ![custCbx-black](/example/custCbx-black.png?raw=true) custCbx-black
* ![custCbx-grey](/example/custCbx-grey.png?raw=true) custCbx-grey
* ![custCbx-white](/example/custCbx-white.png?raw=true) custCbx-white
* ![custCbx-blue](/example/custCbx-blue.png?raw=true) custCbx-blue
* ![custCbx-red](/example/custCbx-red.png?raw=true) custCbx-red
* ![custCbx-violet](/example/custCbx-violet.png?raw=true) custCbx-violet
* ![custCbx-green](/example/custCbx-green.png?raw=true) custCbx-green

You can mix shape / animation / color classes as in this example: ![custCbx-mixed-example](/example/custCbx_mixed-example.gif?raw=true)

Feel free to edit the styles.css and create your own styles!

***Warning: Only one class of each category can be used. In case of multiple classes from a same category, only the first one will be used.***

### Specific actions

* custCbxCheckAll(): check all custom checkboxes on the page
* custCbxUncheckAll(): uncheck all custom checkboxes on the page
* custCbxStatus(*itemId*): return the check state of a checkbox

## Example

``` html
<html>
  <head>
    <link rel="stylesheet" media="screen" href="vendor/custom-checkboxes-master/themes/styles.min.css" type="text/css" >
  </head>
  <body>
    <p>
      <input id="checkbox1" type="checkbox" class="custCbx custCbx-fading">
      <label for="checkbox1">Hit me!</label>
    </p>

    <p>
      <input id="checkbox2" type="checkbox" class="custCbx custCbx-round custCbx-red">
      <label for="checkbox2">Hit me too!</label>
    </p>

    <p>
      <input id="checkbox3" type="checkbox" class="custCbx custCbx-checking" checked>
      <label for="checkbox3">Already checked</label>
    </p>
    
    <script type="text/javascript" src="vendor/custom-checkboxes-master/js/customCheckboxes_1.0.min.js"></script>
    <script>
      custCbx();
    </script>
  </body>
</html>
```

You can find a full [demo here](https://codepen.io/alexisr/pen/VRyZrY). More details on [my blog](https://alx.design/article/14-custom-checkboxes).
