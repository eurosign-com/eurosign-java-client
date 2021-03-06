# swagger-java-client

Eurosign
- API version: 1.0.0
  - Build date: 2020-05-13T10:06:26.547+02:00[Europe/Paris]

This is the documentation of the eurosign API, you can download all of our SDK in this page.


*Automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen)*


## Requirements

Building the API client library requires:
1. Java 1.7+
2. Maven/Gradle

## Installation

To install the API client library to your local Maven repository, simply execute:

```shell
mvn clean install
```

To deploy it to a remote Maven repository instead, configure the settings of the repository and execute:

```shell
mvn clean deploy
```

Refer to the [OSSRH Guide](http://central.sonatype.org/pages/ossrh-guide.html) for more information.

### Maven users

Add this dependency to your project's POM:

```xml
<dependency>
  <groupId>io.swagger</groupId>
  <artifactId>swagger-java-client</artifactId>
  <version>1.5.6</version>
  <scope>compile</scope>
</dependency>
```

### Gradle users

Add this dependency to your project's build file:

```groovy
compile "io.swagger:swagger-java-client:1.5.6"
```

### Others

At first generate the JAR by executing:

```shell
mvn clean package
```

Then manually install the following JARs:

* `target/swagger-java-client-1.5.6.jar`
* `target/lib/*.jar`

## Getting Started

Please follow the [installation](#installation) instruction and execute the following Java code:

```java
import Eurosign.*;
import Eurosign.auth.*;
import io.swagger.client.model.*;
import io.swagger.client.api.SignatureRequestsApi;

import java.io.File;
import java.util.*;

public class SignatureRequestsApiExample {

    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();

        // Configure OAuth2 access token for authorization: eurosign_auth
        OAuth eurosign_auth = (OAuth) defaultClient.getAuthentication("eurosign_auth");
        eurosign_auth.setAccessToken("YOUR ACCESS TOKEN");

        SignatureRequestsApi apiInstance = new SignatureRequestsApi();
        String uuid = "uuid_example"; // String | The signature request UUID
        try {
            apiInstance.cancelSignatureRequests(uuid);
        } catch (ApiException e) {
            System.err.println("Exception when calling SignatureRequestsApi#cancelSignatureRequests");
            e.printStackTrace();
        }
    }
}
import Eurosign.*;
import Eurosign.auth.*;
import io.swagger.client.model.*;
import io.swagger.client.api.SignatureRequestsApi;

import java.io.File;
import java.util.*;

public class SignatureRequestsApiExample {

    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();

        // Configure OAuth2 access token for authorization: eurosign_auth
        OAuth eurosign_auth = (OAuth) defaultClient.getAuthentication("eurosign_auth");
        eurosign_auth.setAccessToken("YOUR ACCESS TOKEN");

        SignatureRequestsApi apiInstance = new SignatureRequestsApi();
        Body body = new Body(); // Body | Input data format
        try {
            InlineResponse2001 result = apiInstance.createSignatureRequest(body);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling SignatureRequestsApi#createSignatureRequest");
            e.printStackTrace();
        }
    }
}
import Eurosign.*;
import Eurosign.auth.*;
import io.swagger.client.model.*;
import io.swagger.client.api.SignatureRequestsApi;

import java.io.File;
import java.util.*;

public class SignatureRequestsApiExample {

    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();

        // Configure OAuth2 access token for authorization: eurosign_auth
        OAuth eurosign_auth = (OAuth) defaultClient.getAuthentication("eurosign_auth");
        eurosign_auth.setAccessToken("YOUR ACCESS TOKEN");

        SignatureRequestsApi apiInstance = new SignatureRequestsApi();
        String uuid = "uuid_example"; // String | Identifiant of a signature request
        try {
            apiInstance.getSignatureRequest(uuid);
        } catch (ApiException e) {
            System.err.println("Exception when calling SignatureRequestsApi#getSignatureRequest");
            e.printStackTrace();
        }
    }
}
import Eurosign.*;
import Eurosign.auth.*;
import io.swagger.client.model.*;
import io.swagger.client.api.SignatureRequestsApi;

import java.io.File;
import java.util.*;

public class SignatureRequestsApiExample {

    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();

        // Configure OAuth2 access token for authorization: eurosign_auth
        OAuth eurosign_auth = (OAuth) defaultClient.getAuthentication("eurosign_auth");
        eurosign_auth.setAccessToken("YOUR ACCESS TOKEN");

        SignatureRequestsApi apiInstance = new SignatureRequestsApi();
        String uuid = "uuid_example"; // String | Identifiant of a signature request
        try {
            apiInstance.getSignatureRequestAuditTrail(uuid);
        } catch (ApiException e) {
            System.err.println("Exception when calling SignatureRequestsApi#getSignatureRequestAuditTrail");
            e.printStackTrace();
        }
    }
}
import Eurosign.*;
import Eurosign.auth.*;
import io.swagger.client.model.*;
import io.swagger.client.api.SignatureRequestsApi;

import java.io.File;
import java.util.*;

public class SignatureRequestsApiExample {

    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();

        // Configure OAuth2 access token for authorization: eurosign_auth
        OAuth eurosign_auth = (OAuth) defaultClient.getAuthentication("eurosign_auth");
        eurosign_auth.setAccessToken("YOUR ACCESS TOKEN");

        SignatureRequestsApi apiInstance = new SignatureRequestsApi();
        String uuid = "uuid_example"; // String | Identifiant of a signature request
        String recipientUuid = "recipientUuid_example"; // String | Identifiant of a recipient
        try {
            apiInstance.getSignatureRequestRecipient(uuid, recipientUuid);
        } catch (ApiException e) {
            System.err.println("Exception when calling SignatureRequestsApi#getSignatureRequestRecipient");
            e.printStackTrace();
        }
    }
}
import Eurosign.*;
import Eurosign.auth.*;
import io.swagger.client.model.*;
import io.swagger.client.api.SignatureRequestsApi;

import java.io.File;
import java.util.*;

public class SignatureRequestsApiExample {

    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();

        // Configure OAuth2 access token for authorization: eurosign_auth
        OAuth eurosign_auth = (OAuth) defaultClient.getAuthentication("eurosign_auth");
        eurosign_auth.setAccessToken("YOUR ACCESS TOKEN");

        SignatureRequestsApi apiInstance = new SignatureRequestsApi();
        String uuid = "uuid_example"; // String | Identifiant of a signature request
        try {
            apiInstance.getSignatureRequestRecipients(uuid);
        } catch (ApiException e) {
            System.err.println("Exception when calling SignatureRequestsApi#getSignatureRequestRecipients");
            e.printStackTrace();
        }
    }
}
import Eurosign.*;
import Eurosign.auth.*;
import io.swagger.client.model.*;
import io.swagger.client.api.SignatureRequestsApi;

import java.io.File;
import java.util.*;

public class SignatureRequestsApiExample {

    public static void main(String[] args) {
        
        SignatureRequestsApi apiInstance = new SignatureRequestsApi();
        try {
            InlineResponse200 result = apiInstance.getSignatureRequests();
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling SignatureRequestsApi#getSignatureRequests");
            e.printStackTrace();
        }
    }
}
import Eurosign.*;
import Eurosign.auth.*;
import io.swagger.client.model.*;
import io.swagger.client.api.SignatureRequestsApi;

import java.io.File;
import java.util.*;

public class SignatureRequestsApiExample {

    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();

        // Configure OAuth2 access token for authorization: eurosign_auth
        OAuth eurosign_auth = (OAuth) defaultClient.getAuthentication("eurosign_auth");
        eurosign_auth.setAccessToken("YOUR ACCESS TOKEN");

        SignatureRequestsApi apiInstance = new SignatureRequestsApi();
        String uuid = "uuid_example"; // String | The signature request UUID
        String senderId = "senderId_example"; // String | The ID of the account_user sending the signature request
        try {
            apiInstance.sendSignatureRequest(uuid, senderId);
        } catch (ApiException e) {
            System.err.println("Exception when calling SignatureRequestsApi#sendSignatureRequest");
            e.printStackTrace();
        }
    }
}
import Eurosign.*;
import Eurosign.auth.*;
import io.swagger.client.model.*;
import io.swagger.client.api.SignatureRequestsApi;

import java.io.File;
import java.util.*;

public class SignatureRequestsApiExample {

    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();

        // Configure OAuth2 access token for authorization: eurosign_auth
        OAuth eurosign_auth = (OAuth) defaultClient.getAuthentication("eurosign_auth");
        eurosign_auth.setAccessToken("YOUR ACCESS TOKEN");

        SignatureRequestsApi apiInstance = new SignatureRequestsApi();
        String uuid = "uuid_example"; // String | The signature request UUID
        Body1 body = new Body1(); // Body1 | Input data format
        try {
            apiInstance.updateSignatureRequest(uuid, body);
        } catch (ApiException e) {
            System.err.println("Exception when calling SignatureRequestsApi#updateSignatureRequest");
            e.printStackTrace();
        }
    }
}
```

## Documentation for API Endpoints

All URIs are relative to *https://api.eurosign.com/v1*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*SignatureRequestsApi* | [**cancelSignatureRequests**](docs/SignatureRequestsApi.md#cancelSignatureRequests) | **POST** /signature-requests/{uuid}/cancel | Cancel a signature requests
*SignatureRequestsApi* | [**createSignatureRequest**](docs/SignatureRequestsApi.md#createSignatureRequest) | **POST** /signature-requests | Create a new signature request
*SignatureRequestsApi* | [**getSignatureRequest**](docs/SignatureRequestsApi.md#getSignatureRequest) | **GET** /signature-requests/{uuid} | Get signature requests test
*SignatureRequestsApi* | [**getSignatureRequestAuditTrail**](docs/SignatureRequestsApi.md#getSignatureRequestAuditTrail) | **GET** /signature-requests/{uuid}/audit-trail | Get the audit report of a signature requests
*SignatureRequestsApi* | [**getSignatureRequestRecipient**](docs/SignatureRequestsApi.md#getSignatureRequestRecipient) | **GET** /signature-requests/{uuid}/recipients/{recipientUuid} | Get a recipient of a signature requests
*SignatureRequestsApi* | [**getSignatureRequestRecipients**](docs/SignatureRequestsApi.md#getSignatureRequestRecipients) | **GET** /signature-requests/{uuid}/recipients | Get recipients of a signature requests
*SignatureRequestsApi* | [**getSignatureRequests**](docs/SignatureRequestsApi.md#getSignatureRequests) | **GET** /signature-requests | Get the list of signature requests
*SignatureRequestsApi* | [**sendSignatureRequest**](docs/SignatureRequestsApi.md#sendSignatureRequest) | **POST** /signature-requests/{uuid}/send | Send a signature requests
*SignatureRequestsApi* | [**updateSignatureRequest**](docs/SignatureRequestsApi.md#updateSignatureRequest) | **PATCH** /signature-requests/{uuid} | Update a signature requests

## Documentation for Models

 - [Body](docs/Body.md)
 - [Body1](docs/Body1.md)
 - [InlineResponse200](docs/InlineResponse200.md)
 - [InlineResponse2001](docs/InlineResponse2001.md)

## Documentation for Authorization

Authentication schemes defined for the API:
### eurosign_auth

- **Type**: OAuth
- **Flow**: implicit
- **Authorization URL**: https://api.eurosign.com/oauth/token
- **Scopes**: 
  - : 


## Recommendation

It's recommended to create an instance of `ApiClient` per thread in a multithreaded environment to avoid any potential issues.

## Author

apiteam@eurosign.com
