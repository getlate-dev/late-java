

# SendConversions200ResponseFailuresInnerCode

## oneOf schemas
* [Integer](Integer.md)
* [String](String.md)

## Example
```java
// Import classes:
import dev.zernio.model.SendConversions200ResponseFailuresInnerCode;
import dev.zernio.model.Integer;
import dev.zernio.model.String;

public class Example {
    public static void main(String[] args) {
        SendConversions200ResponseFailuresInnerCode exampleSendConversions200ResponseFailuresInnerCode = new SendConversions200ResponseFailuresInnerCode();

        // create a new Integer
        Integer exampleInteger = new Integer();
        // set SendConversions200ResponseFailuresInnerCode to Integer
        exampleSendConversions200ResponseFailuresInnerCode.setActualInstance(exampleInteger);
        // to get back the Integer set earlier
        Integer testInteger = (Integer) exampleSendConversions200ResponseFailuresInnerCode.getActualInstance();

        // create a new String
        String exampleString = new String();
        // set SendConversions200ResponseFailuresInnerCode to String
        exampleSendConversions200ResponseFailuresInnerCode.setActualInstance(exampleString);
        // to get back the String set earlier
        String testString = (String) exampleSendConversions200ResponseFailuresInnerCode.getActualInstance();
    }
}
```


