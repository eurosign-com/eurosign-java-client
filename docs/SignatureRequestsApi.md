# SignatureRequestsApi

All URIs are relative to *https://api.eurosign.com/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cancelSignatureRequests**](SignatureRequestsApi.md#cancelSignatureRequests) | **POST** /signature-requests/{uuid}/cancel | Cancel a signature requests
[**createSignatureRequest**](SignatureRequestsApi.md#createSignatureRequest) | **POST** /signature-requests | Create a new signature request
[**getSignatureRequest**](SignatureRequestsApi.md#getSignatureRequest) | **GET** /signature-requests/{uuid} | Get signature requests test
[**getSignatureRequestAuditTrail**](SignatureRequestsApi.md#getSignatureRequestAuditTrail) | **GET** /signature-requests/{uuid}/audit-trail | Get the audit report of a signature requests
[**getSignatureRequestRecipient**](SignatureRequestsApi.md#getSignatureRequestRecipient) | **GET** /signature-requests/{uuid}/recipients/{recipientUuid} | Get a recipient of a signature requests
[**getSignatureRequestRecipients**](SignatureRequestsApi.md#getSignatureRequestRecipients) | **GET** /signature-requests/{uuid}/recipients | Get recipients of a signature requests
[**getSignatureRequests**](SignatureRequestsApi.md#getSignatureRequests) | **GET** /signature-requests | Get the list of signature requests
[**sendSignatureRequest**](SignatureRequestsApi.md#sendSignatureRequest) | **POST** /signature-requests/{uuid}/send | Send a signature requests
[**updateSignatureRequest**](SignatureRequestsApi.md#updateSignatureRequest) | **PATCH** /signature-requests/{uuid} | Update a signature requests

<a name="cancelSignatureRequests"></a>
# **cancelSignatureRequests**
> cancelSignatureRequests(uuid)

Cancel a signature requests

### Example
```java
// Import classes:
//import Eurosign.ApiClient;
//import Eurosign.ApiException;
//import Eurosign.Configuration;
//import Eurosign.auth.*;
//import io.swagger.client.api.SignatureRequestsApi;

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
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uuid** | **String**| The signature request UUID |

### Return type

null (empty response body)

### Authorization

[eurosign_auth](../README.md#eurosign_auth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="createSignatureRequest"></a>
# **createSignatureRequest**
> InlineResponse2001 createSignatureRequest(body)

Create a new signature request

### Example
```java
// Import classes:
//import Eurosign.ApiClient;
//import Eurosign.ApiException;
//import Eurosign.Configuration;
//import Eurosign.auth.*;
//import io.swagger.client.api.SignatureRequestsApi;

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
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Body**](Body.md)| Input data format | [optional]

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

[eurosign_auth](../README.md#eurosign_auth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getSignatureRequest"></a>
# **getSignatureRequest**
> getSignatureRequest(uuid)

Get signature requests test

### Example
```java
// Import classes:
//import Eurosign.ApiClient;
//import Eurosign.ApiException;
//import Eurosign.Configuration;
//import Eurosign.auth.*;
//import io.swagger.client.api.SignatureRequestsApi;

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
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uuid** | **String**| Identifiant of a signature request |

### Return type

null (empty response body)

### Authorization

[eurosign_auth](../README.md#eurosign_auth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="getSignatureRequestAuditTrail"></a>
# **getSignatureRequestAuditTrail**
> getSignatureRequestAuditTrail(uuid)

Get the audit report of a signature requests

### Example
```java
// Import classes:
//import Eurosign.ApiClient;
//import Eurosign.ApiException;
//import Eurosign.Configuration;
//import Eurosign.auth.*;
//import io.swagger.client.api.SignatureRequestsApi;

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
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uuid** | **String**| Identifiant of a signature request |

### Return type

null (empty response body)

### Authorization

[eurosign_auth](../README.md#eurosign_auth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="getSignatureRequestRecipient"></a>
# **getSignatureRequestRecipient**
> getSignatureRequestRecipient(uuid, recipientUuid)

Get a recipient of a signature requests

### Example
```java
// Import classes:
//import Eurosign.ApiClient;
//import Eurosign.ApiException;
//import Eurosign.Configuration;
//import Eurosign.auth.*;
//import io.swagger.client.api.SignatureRequestsApi;

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
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uuid** | **String**| Identifiant of a signature request |
 **recipientUuid** | **String**| Identifiant of a recipient |

### Return type

null (empty response body)

### Authorization

[eurosign_auth](../README.md#eurosign_auth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="getSignatureRequestRecipients"></a>
# **getSignatureRequestRecipients**
> getSignatureRequestRecipients(uuid)

Get recipients of a signature requests

### Example
```java
// Import classes:
//import Eurosign.ApiClient;
//import Eurosign.ApiException;
//import Eurosign.Configuration;
//import Eurosign.auth.*;
//import io.swagger.client.api.SignatureRequestsApi;

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
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uuid** | **String**| Identifiant of a signature request |

### Return type

null (empty response body)

### Authorization

[eurosign_auth](../README.md#eurosign_auth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="getSignatureRequests"></a>
# **getSignatureRequests**
> InlineResponse200 getSignatureRequests()

Get the list of signature requests

Retrieve the list of all the signature requests

### Example
```java
// Import classes:
//import Eurosign.ApiException;
//import io.swagger.client.api.SignatureRequestsApi;


SignatureRequestsApi apiInstance = new SignatureRequestsApi();
try {
    InlineResponse200 result = apiInstance.getSignatureRequests();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SignatureRequestsApi#getSignatureRequests");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="sendSignatureRequest"></a>
# **sendSignatureRequest**
> sendSignatureRequest(uuid, senderId)

Send a signature requests

### Example
```java
// Import classes:
//import Eurosign.ApiClient;
//import Eurosign.ApiException;
//import Eurosign.Configuration;
//import Eurosign.auth.*;
//import io.swagger.client.api.SignatureRequestsApi;

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
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uuid** | **String**| The signature request UUID |
 **senderId** | **String**| The ID of the account_user sending the signature request |

### Return type

null (empty response body)

### Authorization

[eurosign_auth](../README.md#eurosign_auth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="updateSignatureRequest"></a>
# **updateSignatureRequest**
> updateSignatureRequest(uuid, body)

Update a signature requests

### Example
```java
// Import classes:
//import Eurosign.ApiClient;
//import Eurosign.ApiException;
//import Eurosign.Configuration;
//import Eurosign.auth.*;
//import io.swagger.client.api.SignatureRequestsApi;

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
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uuid** | **String**| The signature request UUID |
 **body** | [**Body1**](Body1.md)| Input data format | [optional]

### Return type

null (empty response body)

### Authorization

[eurosign_auth](../README.md#eurosign_auth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

