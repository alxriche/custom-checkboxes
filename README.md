# Custom checkboxes

A light and simple way to custom your form checkboxes

## Project status

**Custom checkboxes 1.0 is released and working.**

This version is stable and should work smoothly on most browsers.

## Installation

Copy this project in your vendor/ directory and initialize it before the closing `</body>` tag and call immediately after the `custCbx()` function:

``` html
  <script type="text/javascript" src="vendor/js/custom-checkboxes/customCheckboxes_1.0.min.js"></script>
  <script>
    custCbx();
  </script>
</body>
```

## Usage

Add the `custCbx` class to all checkboxes to customize.

***Notice: All checkboxes must have an id.***

***Notice: Checkboxes can be prechecked.***

You can add styling classes:

### Manage shape (default: square)
* custCbx-square ![custCbx-square](/example/custCbx-square.png?raw=true)
* custCbx-rounded ![custCbx-rounded](https://raw.githubusercontent.com/alxriche/custom-checkboxes/master/example/custCbx-rounded.png?raw=true)
* custCbx-round ![custCbx-round](https://raw.githubusercontent.com/alxriche/custom-checkboxes/master/example/custCbx-round.png)
* custCbx-tick (mutually exclusive with *animation* class `custCbx-checking`) ![custCbx-tick](https://raw.githubusercontent.com/alxriche/custom-checkboxes/master/example/custCbx-tick.png)

### Manage animation (default: no animation)
* custCbx-fading ![custCbx-fading](https://raw.githubusercontent.com/alxriche/custom-checkboxes/master/example/custCbx-fading.gif)
* custCbx-checking (based on the `custCbx-tick` shape class) ![custCbx-checking](https://raw.githubusercontent.com/alxriche/custom-checkboxes/master/example/custCbx-checking.gif)

### Manage color (default: black)
* custCbx-black ![custCbx-black](https://raw.githubusercontent.com/alxriche/custom-checkboxes/master/example/custCbx-black.png)
* custCbx-grey ![custCbx-grey](https://raw.githubusercontent.com/alxriche/custom-checkboxes/master/example/custCbx-grey.png)
* custCbx-white ![custCbx-white](https://raw.githubusercontent.com/alxriche/custom-checkboxes/master/example/custCbx-white.png)
* custCbx-blue ![custCbx-blue](https://raw.githubusercontent.com/alxriche/custom-checkboxes/master/example/custCbx-blue.png)
* custCbx-red ![custCbx-red](https://raw.githubusercontent.com/alxriche/custom-checkboxes/master/example/custCbx-red.png)
* custCbx-violet ![custCbx-violet](https://raw.githubusercontent.com/alxriche/custom-checkboxes/master/example/custCbx-violet.png)
* custCbx-green ![custCbx-green](https://raw.githubusercontent.com/alxriche/custom-checkboxes/master/example/custCbx-green.png)

***Warning: Only one class of each category can be used. In case of multiple classes from a same category, only the first one will be used.***

## Example

``` html
<html>
  <head>
    ...
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
    
    <script type="text/javascript" src="vendor/js/custom-checkboxes/customCheckboxes_1.0.min.js"></script>
    <script>
      custCbx();
    </script>
  </body>
</html>
```

You can find a full [demo here](). More details on [my blog](https://alx.design/article/14-custom-checkboxes).
