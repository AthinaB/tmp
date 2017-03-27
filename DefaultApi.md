# BloodDonorRegistryForDonorsApplication.DefaultApi

All URIs are relative to *https://service.blooddonorregistry.gr*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getLocale**](DefaultApi.md#getLocale) | **GET** /locale/{lang}.json | Get i18n json
[**getUserData**](DefaultApi.md#getUserData) | **GET** /blood-donor-registry-web-public/rest/authentication/logged-on | Retrieve user data
[**tba2**](DefaultApi.md#tba2) | **GET** /blood-donor-registry-web-public/rest/blooddonor/8616993 | tba


<a name="getLocale"></a>
# **getLocale**
> Object getLocale(lang)

Get i18n json

All the texts that the UI needs to display in key-value pairs.  No login is required for this request.  Available languages:  - English : en - Greek : el 

### Example
```javascript
var BloodDonorRegistryForDonorsApplication = require('blood_donor_registry_for_donors_application');

var apiInstance = new BloodDonorRegistryForDonorsApplication.DefaultApi();

var lang = "lang_example"; // String | 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.getLocale(lang, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lang** | **String**|  | 

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json, text/html

<a name="getUserData"></a>
# **getUserData**
> User getUserData(xAuthToken)

Retrieve user data

Se Login is required. 

### Example
```javascript
var BloodDonorRegistryForDonorsApplication = require('blood_donor_registry_for_donors_application');

var apiInstance = new BloodDonorRegistryForDonorsApplication.DefaultApi();

var xAuthToken = "xAuthToken_example"; // String | authentication data


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.getUserData(xAuthToken, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **xAuthToken** | **String**| authentication data | 

### Return type

[**User**](User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json

<a name="tba2"></a>
# **tba2**
> Object tba2()

tba

tba

### Example
```javascript
var BloodDonorRegistryForDonorsApplication = require('blood_donor_registry_for_donors_application');

var apiInstance = new BloodDonorRegistryForDonorsApplication.DefaultApi();

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.tba2(callback);
```

### Parameters
This endpoint does not need any parameter.

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/plain
 - **Accept**: application/json, text/html

