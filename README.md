

A simple script for simulating raindrops falling on a glass surface.

For demos and more information see the [project page](http://maroslaw.github.io/rainyday.js/).

### How to use:

```js
var engine = new RainyDay({
    image: element,         // Image element
                            // This value is required
    parentElement: someDiv, // Element to be used as a parent for the canvas
                            // If not provided assuming the 'body' element
    crop: [0, 0, 50, 60],   // Coordinates if only a part of the image should be used
                            // If not provided entire image will be used
    blur: 10,               // Defines blur due to rain effect
                            // Assuming 10 if not provided
                            // Use 0 value to disable the blur
    opacity: 1              // Opacity of rain drops
                            // Assuming 1 if not provided
});
engine.rain(
    [
        [1, 0, 20],         // add 20 drops of size 1...
        [3, 3, 1]           // ... and 1 drop of size from 3 - 6 ...
    ],                       
    100);                   // ... every 100ms
```
