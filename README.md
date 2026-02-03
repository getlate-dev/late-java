# Late Java SDK

Official Java client library for the [Late API](https://docs.getlate.dev) - Schedule and manage social media posts across multiple platforms.

## Installation

### Maven

```xml
<dependency>
  <groupId>dev.getlate</groupId>
  <artifactId>late-sdk</artifactId>
  <version>0.1.0</version>
</dependency>
```

### Gradle

```groovy
implementation 'dev.getlate:late-sdk:0.1.0'
```

## Quick Start

```java
import dev.getlate.ApiClient;
import dev.getlate.api.AccountsApi;
import dev.getlate.api.PostsApi;
import dev.getlate.model.*;

public class Example {
    public static void main(String[] args) {
        ApiClient client = new ApiClient();
        client.setApiKey("YOUR_API_KEY");

        // List accounts
        AccountsApi accountsApi = new AccountsApi(client);
        List<Account> accounts = accountsApi.listAccounts();
        System.out.println(accounts);

        // Create a post
        PostsApi postsApi = new PostsApi(client);
        CreatePostRequest request = new CreatePostRequest()
            .content("Hello from Java!")
            .publishNow(true);
        Post post = postsApi.createPost(request);
    }
}
```

## Documentation

- [API Reference](https://docs.getlate.dev/api-reference)
- [Getting Started Guide](https://docs.getlate.dev/quickstart)

## License

MIT
