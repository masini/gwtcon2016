##  Errai Framework

* Dagger 2 is ligther and can wire applications like Errai CDI does, but...
* ...with Errai CDI we use the same programming model on client code and server code
* We also used a lot "Errai Navigation", "Errai Security" and "Errai JAX-RS"

Note:

Why we use Errai ? 

Is an historical choice, when we started we could use Errai or directly GIN. Today GIN has been replaced by Dagger2 
which is very lightweight and yet use APT to wire everything, but we decided to remain on Errai because:

1) The API model is based on the CDI specs, which are used in our server side code
   Doing this we can have the same language and the same programming model on client and server code
2) We don't use only injection, as we said before we use a lot Errai Navigation, Security and JAX-RS
 
The only drawback in Errai is due to the mix of its generated code and GWT caches, sometimes we need to clean 
everything because suddenly things stop working, injections stops and you don't know if you wrote something wrong or
if again you are in this condition.
