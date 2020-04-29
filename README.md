# web_snippets
A summary of the most useful code snippets and frameworks for web developement 



- https://github.com/TrueValentine/material-photo-gallery

  ```js
  var elem = document.querySelector('.m-p-g');
  
  document.addEventListener('DOMContentLoaded', function() {
      var gallery = new MaterialPhotoGallery(elem);
  });
  
  document.onkeydown = checkKey;
  
  function checkKey(e) {
  
      e = e || window.event;
  
      if (e.keyCode == '38') {
          // up arrow
      }
      else if (e.keyCode == '40') {
          // down arrow
      }
      else if (e.keyCode == '37') {
         // left arrow
         document.querySelector('.m-p-g__controls-arrow--prev').click()
      }
      else if (e.keyCode == '39') {
         // right arrow
         document.querySelector('.m-p-g__controls-arrow--next').click()
      }
      else if (e.keyCode == '27') {
          // escape key
          document.querySelector('.m-p-g__controls-close').click()
      }
  }
  ```

  --> **script.js**