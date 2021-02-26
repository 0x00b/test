# TestProto.TestApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**testEcho**](TestApi.md#testEcho) | **POST** /v1/example/echo/{userId} | curl &#39;localhost:8080/v1/example/echo/userid123?appId&#x3D;1&#39; -XPOST  -H \&quot;Content-Type: application/json\&quot; -d &#39;{\&quot;value\&quot;:\&quot;v1\&quot;}&#39;



## testEcho

> TestEchoResp testEcho(userId, body, opts)

curl &#39;localhost:8080/v1/example/echo/userid123?appId&#x3D;1&#39; -XPOST  -H \&quot;Content-Type: application/json\&quot; -d &#39;{\&quot;value\&quot;:\&quot;v1\&quot;}&#39;

### Example

```javascript
import TestProto from 'test_proto';

let apiInstance = new TestProto.TestApi();
let userId = "userId_example"; // String | mapped to the URL, appId
let body = new TestProto.TestRequestBody(); // TestRequestBody | mapped to the body
let opts = {
  'appId': "appId_example" // String | not bind, mapped to the query, userId.
};
apiInstance.testEcho(userId, body, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **String**| mapped to the URL, appId | 
 **body** | [**TestRequestBody**](TestRequestBody.md)| mapped to the body | 
 **appId** | **String**| not bind, mapped to the query, userId. | [optional] 

### Return type

[**TestEchoResp**](TestEchoResp.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

