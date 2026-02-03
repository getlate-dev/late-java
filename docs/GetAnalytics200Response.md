

# GetAnalytics200Response

## oneOf schemas
* [AnalyticsListResponse](AnalyticsListResponse.md)
* [AnalyticsSinglePostResponse](AnalyticsSinglePostResponse.md)

## Example
```java
// Import classes:
import dev.getlate.model.GetAnalytics200Response;
import dev.getlate.model.AnalyticsListResponse;
import dev.getlate.model.AnalyticsSinglePostResponse;

public class Example {
    public static void main(String[] args) {
        GetAnalytics200Response exampleGetAnalytics200Response = new GetAnalytics200Response();

        // create a new AnalyticsListResponse
        AnalyticsListResponse exampleAnalyticsListResponse = new AnalyticsListResponse();
        // set GetAnalytics200Response to AnalyticsListResponse
        exampleGetAnalytics200Response.setActualInstance(exampleAnalyticsListResponse);
        // to get back the AnalyticsListResponse set earlier
        AnalyticsListResponse testAnalyticsListResponse = (AnalyticsListResponse) exampleGetAnalytics200Response.getActualInstance();

        // create a new AnalyticsSinglePostResponse
        AnalyticsSinglePostResponse exampleAnalyticsSinglePostResponse = new AnalyticsSinglePostResponse();
        // set GetAnalytics200Response to AnalyticsSinglePostResponse
        exampleGetAnalytics200Response.setActualInstance(exampleAnalyticsSinglePostResponse);
        // to get back the AnalyticsSinglePostResponse set earlier
        AnalyticsSinglePostResponse testAnalyticsSinglePostResponse = (AnalyticsSinglePostResponse) exampleGetAnalytics200Response.getActualInstance();
    }
}
```


