##  Target

* A coherent layout <!-- .element: class="fragment" data-fragment-index="1" -->
* Integration with an external provisioning system for user and application data <!-- .element: class="fragment" data-fragment-index="2" --> 
* Simplified REST call <!-- .element: class="fragment" data-fragment-index="3" -->
* GWT Widgets that let the developer ignore the underlying HTML5/CSS <!-- .element: class="fragment" data-fragment-index="4" -->

This was done gluing together some carefully chosen available frameworks. <!-- .element: class="fragment" data-fragment-index="5" --> 

Note:

As I said, we identified these objectives for our metaframework:

A coherent layout, complete of all the necessary elements, I will say more about this later //
Automatic integration with backend subsystem, in particular user provisioning and bootstrap application data //
A simple alternative to gwt-rpc to call REST end-point
Plain old GWT Widgets that let the developer write the user interface without worrying too much about what HTML will be generated, but assuring us that the layout and style will be preserved

To do this we selected some frameworks available in the open source GWT space and we integrated them for the end-user developer
