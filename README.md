LinkedIn-Auto-Endorse
=====================

Copy and paste the following script in the console while the endorsement box showing.

```javascript
var timeout = 1000;
var action = function() {
    // Loop the endorse buttons
    $('.endorse-action').each(function(index, value){
      setTimeout(function() {
        $(value).trigger('click', true );
        console.log($('.endorse-action').parent().find('.endorse-question strong:eq(0)').html() + ' knows ' + $('.endorse-action').parent().find('.endorse-question strong:eq(1)').html());
      }, 1500);
    });
    setTimeout(action, timeout);
};
action();
```
