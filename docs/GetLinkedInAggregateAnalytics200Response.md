

# GetLinkedInAggregateAnalytics200Response

## oneOf schemas
* [LinkedInAggregateAnalyticsDailyResponse](LinkedInAggregateAnalyticsDailyResponse.md)
* [LinkedInAggregateAnalyticsTotalResponse](LinkedInAggregateAnalyticsTotalResponse.md)

## Example
```java
// Import classes:
import dev.getlate.model.GetLinkedInAggregateAnalytics200Response;
import dev.getlate.model.LinkedInAggregateAnalyticsDailyResponse;
import dev.getlate.model.LinkedInAggregateAnalyticsTotalResponse;

public class Example {
    public static void main(String[] args) {
        GetLinkedInAggregateAnalytics200Response exampleGetLinkedInAggregateAnalytics200Response = new GetLinkedInAggregateAnalytics200Response();

        // create a new LinkedInAggregateAnalyticsDailyResponse
        LinkedInAggregateAnalyticsDailyResponse exampleLinkedInAggregateAnalyticsDailyResponse = new LinkedInAggregateAnalyticsDailyResponse();
        // set GetLinkedInAggregateAnalytics200Response to LinkedInAggregateAnalyticsDailyResponse
        exampleGetLinkedInAggregateAnalytics200Response.setActualInstance(exampleLinkedInAggregateAnalyticsDailyResponse);
        // to get back the LinkedInAggregateAnalyticsDailyResponse set earlier
        LinkedInAggregateAnalyticsDailyResponse testLinkedInAggregateAnalyticsDailyResponse = (LinkedInAggregateAnalyticsDailyResponse) exampleGetLinkedInAggregateAnalytics200Response.getActualInstance();

        // create a new LinkedInAggregateAnalyticsTotalResponse
        LinkedInAggregateAnalyticsTotalResponse exampleLinkedInAggregateAnalyticsTotalResponse = new LinkedInAggregateAnalyticsTotalResponse();
        // set GetLinkedInAggregateAnalytics200Response to LinkedInAggregateAnalyticsTotalResponse
        exampleGetLinkedInAggregateAnalytics200Response.setActualInstance(exampleLinkedInAggregateAnalyticsTotalResponse);
        // to get back the LinkedInAggregateAnalyticsTotalResponse set earlier
        LinkedInAggregateAnalyticsTotalResponse testLinkedInAggregateAnalyticsTotalResponse = (LinkedInAggregateAnalyticsTotalResponse) exampleGetLinkedInAggregateAnalytics200Response.getActualInstance();
    }
}
```


