##  Why not the sexy XXX framework ?

Here a snippet of code using ProductiveGWT

```Java
@MenuEntry(text = "Catalogue") //Integration with GUI and Security
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
