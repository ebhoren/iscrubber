iScrubber
=========

jQuery plugin that mimics iPhoto's picture scrubbing feature.

[See demo page](http://skarface.github.io/iscrubber/)

##### 1.2.0
* Added option to choose the mouse direction that show the items

### Minimal Setup

* Create the element structure with pictures

`````html
  <ul class="scrubber">
    <li><img src="images/image1.png"></li>
    <li><img src="images/image2.png"></li>
    <li><img src="images/image3.png"></li>
    <li><img src="images/image4.png"></li>
  </ul>
`````

* Add this line to your CSS

`````css
  ul.scrubber li {display: none;}
`````

* Add jQuery and iScrubber libs

`````html
  <script src="http://ajax.googleapis.com/ajax/libs/jquery/2.0.0/jquery.min.js"></script>
  <script src="lib/jquery.iscrubber.min.js"></script>
`````

* Initialize the plugin

`````javascript
  $(".scrubber").iscrubber();
`````

* Customize it

`````javascript
  $(".scrubber").iscrubber({
    showItem: 1, // the element (li) to show first; 1 based index
    leaveToFirst: true, // come back the the first element when mouse leaves scrubbing area
    direction: "horizontal" // use to specified the direction that mouse takes to show the items
  });
`````
