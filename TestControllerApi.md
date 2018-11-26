# TestControllerApi

All URIs are relative to *https://localhost:8090*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getTestStringUsingGET**](TestControllerApi.md#getTestStringUsingGET) | **GET** /service/hi | getTestString


<a name="getTestStringUsingGET"></a>
# **getTestStringUsingGET**
> String getTestStringUsingGET()

getTestString

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.TestControllerApi;


TestControllerApi apiInstance = new TestControllerApi();
try {
    String result = apiInstance.getTestStringUsingGET();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TestControllerApi#getTestStringUsingGET");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

