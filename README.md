
```| jquery.horizonScroll.js - Horizontal Scrolling (Paging) Websites | Demo| Usage |
| :---         |     :---:      |          ---: |
|This is a jQuery plugin which allows for websites to page(scroll by set width) left and right horizontally. Horizontal scroll sites offer a new and unique way to develope sites! Check it out and give feedback! THX  | Click here for the [demo](https://fraules.github.io/DemoTest)   |Initial usage. All elements specified by the selector become a page.
```javascript
$('selector').horizon();
```

If you do not want to use jquery.swipeTouch.js for swipe left and right:
```javascript
$('selector').horizon({swipe: false});
```

Additional plugin options and their default values:
```javascript
$.fn.horizon.defaults = {
    scrollTimeout: null,
    scrollEndDelay: 250,
    scrollDuration: 400,
    i: 0,
    limit: 0,
    docWidth: 0,
    sections: null,
    swipe: true,
    fnCallback: function (i) {}
};   |
| git diff     | git diff       | ```javascript
$(document).horizon('scrollRight');
$(document).horizon('scrollLeft');

// As of 1.1.0, i can be an integer with or without quotes in order to scroll to an index.
// Or i can be a string of an element id to scroll to.
$(document).horizon('scrollTo', i);      |

