

# SocialAccountProfileId

## oneOf schemas
* [Profile](Profile.md)
* [String](String.md)

## Example
```java
// Import classes:
import dev.getlate.model.SocialAccountProfileId;
import dev.getlate.model.Profile;
import dev.getlate.model.String;

public class Example {
    public static void main(String[] args) {
        SocialAccountProfileId exampleSocialAccountProfileId = new SocialAccountProfileId();

        // create a new Profile
        Profile exampleProfile = new Profile();
        // set SocialAccountProfileId to Profile
        exampleSocialAccountProfileId.setActualInstance(exampleProfile);
        // to get back the Profile set earlier
        Profile testProfile = (Profile) exampleSocialAccountProfileId.getActualInstance();

        // create a new String
        String exampleString = new String();
        // set SocialAccountProfileId to String
        exampleSocialAccountProfileId.setActualInstance(exampleString);
        // to get back the String set earlier
        String testString = (String) exampleSocialAccountProfileId.getActualInstance();
    }
}
```


