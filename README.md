# jquery-izoomify
jquery-izoomify is an image zoom plugin. It creates a flawless zoom effect to your images. Inspired by [jquery-zoom](http://www.jacklmoore.com/zoom) plugin.

``jquery-izoomify v1.0`` requires ``jQuery 1.8+``

# Settings
- ``target`` - Parent container. Default is false.
- ``url`` - Url of image to display on hover. Default is false.
- ``magnify`` - Image zooming or magnification. Default is 1.2.
- ``touch`` - Interaction with touch events. Default is true.
- ``duration`` - Speed of image zooming in/out. Default is 120.
- ``callback`` - Function to be called once loaded. Default false.
 
# Markup
##### Default
---
```html
<div class="target">
    <img src="path/to/image.jpg" />
</div>
```
```js
<script>
$(document).ready(function() {
   $('.target').izoomify(); 
});
<script>
```
##### Data Attribute
---
```html
<div class="target">
    <img src="low-res/image.jpg" 
        data-izoomify-url="hi-res/hover.jpg" 
        data-izoomify-magnify="1.8" 
        data-izoomify-duration="300" />
</div>
```
```js
<script>
$(document).ready(function() {
   $('.target').izoomify(); 
});
<script>
```
##### Javascript
---
```html
<div class="target">
    <img src="low-res/image.jpg" />
</div>
```
```js
<script>
$(document).ready(function() {
   $('.target').izoomify({
       url: "hi-res/hover.jpg",
       magnify: 2.75,
       duration: 450,
       callback: function () {
           // your code here...
       }
   }); 
});
<script>
```

## License

jquery-izoomify is released under the MIT Licence.
