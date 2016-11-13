##  GWT 2.8

* Java 8 is cool but....

    * 2.8 compile time is higher than in 2.7 <!-- .element: class="fragment" -->
    * More memory usage (+80%) <!-- .element: class="fragment" -->
    * Variables name now are even more cryptically and still no support from Source Maps <!-- .element: class="fragment" --> 

Note: 

Having worked now a lot with GWT 2.8 now we can say that having the same Java version client/server is again a plus, we
had to survive a lot with Java 8 server-side and Java 6/7 on the client.

We don't use lambda a lot because thanks to UI Binder events are managed by instance methods.

We also have an opinion of what must be improved:

* We measured higher compile time in the same application upgrading from 2.7 to 2.8
* We also measured higher memory usage
* Super Dev Mode is cool but debugging is difficult, most of this come from the local variables which are not included in Source Maps
  GWT 2.8 put also the package and class name inside the variable name, along with dollars, underscore and numbers, 
  finding the correct variable to inspect is not easy 

