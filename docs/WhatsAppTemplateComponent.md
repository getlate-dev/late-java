

# WhatsAppTemplateComponent

## oneOf schemas
* [WhatsAppBodyComponent](WhatsAppBodyComponent.md)
* [WhatsAppButtonsComponent](WhatsAppButtonsComponent.md)
* [WhatsAppFooterComponent](WhatsAppFooterComponent.md)
* [WhatsAppHeaderComponent](WhatsAppHeaderComponent.md)

## Example
```java
// Import classes:
import dev.zernio.model.WhatsAppTemplateComponent;
import dev.zernio.model.WhatsAppBodyComponent;
import dev.zernio.model.WhatsAppButtonsComponent;
import dev.zernio.model.WhatsAppFooterComponent;
import dev.zernio.model.WhatsAppHeaderComponent;

public class Example {
    public static void main(String[] args) {
        WhatsAppTemplateComponent exampleWhatsAppTemplateComponent = new WhatsAppTemplateComponent();

        // create a new WhatsAppBodyComponent
        WhatsAppBodyComponent exampleWhatsAppBodyComponent = new WhatsAppBodyComponent();
        // set WhatsAppTemplateComponent to WhatsAppBodyComponent
        exampleWhatsAppTemplateComponent.setActualInstance(exampleWhatsAppBodyComponent);
        // to get back the WhatsAppBodyComponent set earlier
        WhatsAppBodyComponent testWhatsAppBodyComponent = (WhatsAppBodyComponent) exampleWhatsAppTemplateComponent.getActualInstance();

        // create a new WhatsAppButtonsComponent
        WhatsAppButtonsComponent exampleWhatsAppButtonsComponent = new WhatsAppButtonsComponent();
        // set WhatsAppTemplateComponent to WhatsAppButtonsComponent
        exampleWhatsAppTemplateComponent.setActualInstance(exampleWhatsAppButtonsComponent);
        // to get back the WhatsAppButtonsComponent set earlier
        WhatsAppButtonsComponent testWhatsAppButtonsComponent = (WhatsAppButtonsComponent) exampleWhatsAppTemplateComponent.getActualInstance();

        // create a new WhatsAppFooterComponent
        WhatsAppFooterComponent exampleWhatsAppFooterComponent = new WhatsAppFooterComponent();
        // set WhatsAppTemplateComponent to WhatsAppFooterComponent
        exampleWhatsAppTemplateComponent.setActualInstance(exampleWhatsAppFooterComponent);
        // to get back the WhatsAppFooterComponent set earlier
        WhatsAppFooterComponent testWhatsAppFooterComponent = (WhatsAppFooterComponent) exampleWhatsAppTemplateComponent.getActualInstance();

        // create a new WhatsAppHeaderComponent
        WhatsAppHeaderComponent exampleWhatsAppHeaderComponent = new WhatsAppHeaderComponent();
        // set WhatsAppTemplateComponent to WhatsAppHeaderComponent
        exampleWhatsAppTemplateComponent.setActualInstance(exampleWhatsAppHeaderComponent);
        // to get back the WhatsAppHeaderComponent set earlier
        WhatsAppHeaderComponent testWhatsAppHeaderComponent = (WhatsAppHeaderComponent) exampleWhatsAppTemplateComponent.getActualInstance();
    }
}
```


