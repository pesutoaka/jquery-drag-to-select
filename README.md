# jQuery.dragToSelect
Use this plug-in to allow your users to select certain elements by dragging a "select box". Works very similar to how you can drag-n-select files and folders in most OS:es.

Installation
------------

### npm

```
npm install jquery-drag-to-select --save
```

### bower

```
bower install jquery-drag-to-select --save
```

How To Use
----------

Initialize:
$(selector).dragToSelect(parameters);

Disable:
$(selector).dragToSelect('disable');

Enable:
$(selector).dragToSelect('enable');


Parameters:

* className: 'jquery-drag-to-select',
* activeClass: 'active',
* disabledClass: 'disabled',
* selectedClass: 'selected',
* scrollTH: 10,
* percentCovered: 25,
* selectables: false,
* autoScroll: false,
* selectOnMove: false,
* onShow: function () {return true;},
* onHide: function () {return true;},
* onRefresh: function () {return true;}


This Fork
---------
Forked from <http://andreaslagerkvist.com/jquery/drag-to-select/>

### Performance improvements:

* Event handlers for mousemove and mouseup attached on selection start and removed at selection end.


### Feature improvementes:

* Better scroll-bar detection, bassed in innerWidth and innerHeight
* the select box is not freezed when mouse go out of the selectable area
* the position of select area is not broken when the offset of selection area is changed.
* minimized files


### Bugs fixed:

* now working with jQuery in noConflict mode
