

# UploadWhatsAppFlowJsonRequestFlowJson

The Flow JSON content. Pass as a JSON object or a JSON string.

## oneOf schemas
* [Object](Object.md)
* [String](String.md)

## Example
```java
// Import classes:
import dev.zernio.model.UploadWhatsAppFlowJsonRequestFlowJson;
import dev.zernio.model.Object;
import dev.zernio.model.String;

public class Example {
    public static void main(String[] args) {
        UploadWhatsAppFlowJsonRequestFlowJson exampleUploadWhatsAppFlowJsonRequestFlowJson = new UploadWhatsAppFlowJsonRequestFlowJson();

        // create a new Object
        Object exampleObject = new Object();
        // set UploadWhatsAppFlowJsonRequestFlowJson to Object
        exampleUploadWhatsAppFlowJsonRequestFlowJson.setActualInstance(exampleObject);
        // to get back the Object set earlier
        Object testObject = (Object) exampleUploadWhatsAppFlowJsonRequestFlowJson.getActualInstance();

        // create a new String
        String exampleString = new String();
        // set UploadWhatsAppFlowJsonRequestFlowJson to String
        exampleUploadWhatsAppFlowJsonRequestFlowJson.setActualInstance(exampleString);
        // to get back the String set earlier
        String testString = (String) exampleUploadWhatsAppFlowJsonRequestFlowJson.getActualInstance();
    }
}
```


