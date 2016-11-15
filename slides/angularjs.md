##  Why not the sexy XXX framework ?

Here a snippet of code using ProductiveGWT
<!-- .element: class="fragment" data-fragment-index="1" -->

```Java
@MenuEntry(text = "Catalogue") //Integration with GUI...
@RestrictedAccess(roles = SecurityRoles.RESPONSABILE) ///...and Security
@Page // Navigation integrated with browser history
public class CataloguePage extends AbstractRicercaView<Catalogue> {

    // Declarative and type-safe UI-Binder
    interface Binder extends UiBinder<VerticalPanel, CataloguePage> {
        Binder INSTANCE = GWT.create(Binder.class);
    }

    @Inject // Service call interface
    Caller<CatalogueService> catalogueServiceCaller; 
    
    // My Business code
``` 
<!-- .element: class="fragment" data-fragment-index="1" -->

Note:

But after 10 years why we decided to remain on GWT with all these cool framework available ?

The answer is in this snippet of code, where I have comndensed some key concept:

* The first annotation is used by our APT generator to create the correct layout and to integrate into the security system
* The second is an Erray Navigation annotation, used to include this widget in the generation of classes needed for the navigation subsystem
* Then we have plain old good UI Binder, in that type-safe XML we declare GWT-Material widgets
* Finally that to Errai CDI we inject an Errai JAX-RS automatically generated proxy to a REST endpoint

