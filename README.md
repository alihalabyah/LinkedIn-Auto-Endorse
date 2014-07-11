LinkedIn-Auto-Endorse
=====================

Copy and paste the script in the console while the endorsement box showing 

```javascript
var timeout = 1000;
var action = function() {
    // Loop the endorse buttons
    $('.endorse-action').each(function(index, value){
      setTimeout(function() {$(value).trigger('click', true );}, 1500);
    });
    setTimeout(action, timeout);
};
action();
```
