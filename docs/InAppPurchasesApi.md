# openapi_client.InAppPurchasesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**in_app_purchases_get_instance**](InAppPurchasesApi.md#in_app_purchases_get_instance) | **GET** /v1/inAppPurchases/{id} | 
[**in_app_purchases_v2_app_store_review_screenshot_get_to_one_related**](InAppPurchasesApi.md#in_app_purchases_v2_app_store_review_screenshot_get_to_one_related) | **GET** /v2/inAppPurchases/{id}/appStoreReviewScreenshot | 
[**in_app_purchases_v2_app_store_review_screenshot_get_to_one_relationship**](InAppPurchasesApi.md#in_app_purchases_v2_app_store_review_screenshot_get_to_one_relationship) | **GET** /v2/inAppPurchases/{id}/relationships/appStoreReviewScreenshot | 
[**in_app_purchases_v2_content_get_to_one_related**](InAppPurchasesApi.md#in_app_purchases_v2_content_get_to_one_related) | **GET** /v2/inAppPurchases/{id}/content | 
[**in_app_purchases_v2_content_get_to_one_relationship**](InAppPurchasesApi.md#in_app_purchases_v2_content_get_to_one_relationship) | **GET** /v2/inAppPurchases/{id}/relationships/content | 
[**in_app_purchases_v2_create_instance**](InAppPurchasesApi.md#in_app_purchases_v2_create_instance) | **POST** /v2/inAppPurchases | 
[**in_app_purchases_v2_delete_instance**](InAppPurchasesApi.md#in_app_purchases_v2_delete_instance) | **DELETE** /v2/inAppPurchases/{id} | 
[**in_app_purchases_v2_get_instance**](InAppPurchasesApi.md#in_app_purchases_v2_get_instance) | **GET** /v2/inAppPurchases/{id} | 
[**in_app_purchases_v2_iap_price_schedule_get_to_one_related**](InAppPurchasesApi.md#in_app_purchases_v2_iap_price_schedule_get_to_one_related) | **GET** /v2/inAppPurchases/{id}/iapPriceSchedule | 
[**in_app_purchases_v2_iap_price_schedule_get_to_one_relationship**](InAppPurchasesApi.md#in_app_purchases_v2_iap_price_schedule_get_to_one_relationship) | **GET** /v2/inAppPurchases/{id}/relationships/iapPriceSchedule | 
[**in_app_purchases_v2_images_get_to_many_related**](InAppPurchasesApi.md#in_app_purchases_v2_images_get_to_many_related) | **GET** /v2/inAppPurchases/{id}/images | 
[**in_app_purchases_v2_images_get_to_many_relationship**](InAppPurchasesApi.md#in_app_purchases_v2_images_get_to_many_relationship) | **GET** /v2/inAppPurchases/{id}/relationships/images | 
[**in_app_purchases_v2_in_app_purchase_availability_get_to_one_related**](InAppPurchasesApi.md#in_app_purchases_v2_in_app_purchase_availability_get_to_one_related) | **GET** /v2/inAppPurchases/{id}/inAppPurchaseAvailability | 
[**in_app_purchases_v2_in_app_purchase_availability_get_to_one_relationship**](InAppPurchasesApi.md#in_app_purchases_v2_in_app_purchase_availability_get_to_one_relationship) | **GET** /v2/inAppPurchases/{id}/relationships/inAppPurchaseAvailability | 
[**in_app_purchases_v2_in_app_purchase_localizations_get_to_many_related**](InAppPurchasesApi.md#in_app_purchases_v2_in_app_purchase_localizations_get_to_many_related) | **GET** /v2/inAppPurchases/{id}/inAppPurchaseLocalizations | 
[**in_app_purchases_v2_in_app_purchase_localizations_get_to_many_relationship**](InAppPurchasesApi.md#in_app_purchases_v2_in_app_purchase_localizations_get_to_many_relationship) | **GET** /v2/inAppPurchases/{id}/relationships/inAppPurchaseLocalizations | 
[**in_app_purchases_v2_price_points_get_to_many_related**](InAppPurchasesApi.md#in_app_purchases_v2_price_points_get_to_many_related) | **GET** /v2/inAppPurchases/{id}/pricePoints | 
[**in_app_purchases_v2_price_points_get_to_many_relationship**](InAppPurchasesApi.md#in_app_purchases_v2_price_points_get_to_many_relationship) | **GET** /v2/inAppPurchases/{id}/relationships/pricePoints | 
[**in_app_purchases_v2_promoted_purchase_get_to_one_related**](InAppPurchasesApi.md#in_app_purchases_v2_promoted_purchase_get_to_one_related) | **GET** /v2/inAppPurchases/{id}/promotedPurchase | 
[**in_app_purchases_v2_promoted_purchase_get_to_one_relationship**](InAppPurchasesApi.md#in_app_purchases_v2_promoted_purchase_get_to_one_relationship) | **GET** /v2/inAppPurchases/{id}/relationships/promotedPurchase | 
[**in_app_purchases_v2_update_instance**](InAppPurchasesApi.md#in_app_purchases_v2_update_instance) | **PATCH** /v2/inAppPurchases/{id} | 


# **in_app_purchases_get_instance**
> InAppPurchaseResponse in_app_purchases_get_instance(id, fields_in_app_purchases=fields_in_app_purchases, include=include, limit_apps=limit_apps)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_response import InAppPurchaseResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_in_app_purchases = ['fields_in_app_purchases_example'] # List[str] | the fields to include for returned resources of type inAppPurchases (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_apps = 56 # int | maximum number of related apps returned (when they are included) (optional)

    try:
        api_response = api_instance.in_app_purchases_get_instance(id, fields_in_app_purchases=fields_in_app_purchases, include=include, limit_apps=limit_apps)
        print("The response of InAppPurchasesApi->in_app_purchases_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_in_app_purchases** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchases | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_apps** | **int**| maximum number of related apps returned (when they are included) | [optional] 

### Return type

[**InAppPurchaseResponse**](InAppPurchaseResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Single InAppPurchase |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_app_store_review_screenshot_get_to_one_related**
> InAppPurchaseAppStoreReviewScreenshotResponse in_app_purchases_v2_app_store_review_screenshot_get_to_one_related(id, fields_in_app_purchase_app_store_review_screenshots=fields_in_app_purchase_app_store_review_screenshots, fields_in_app_purchases=fields_in_app_purchases, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_app_store_review_screenshot_response import InAppPurchaseAppStoreReviewScreenshotResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_in_app_purchase_app_store_review_screenshots = ['fields_in_app_purchase_app_store_review_screenshots_example'] # List[str] | the fields to include for returned resources of type inAppPurchaseAppStoreReviewScreenshots (optional)
    fields_in_app_purchases = ['fields_in_app_purchases_example'] # List[str] | the fields to include for returned resources of type inAppPurchases (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.in_app_purchases_v2_app_store_review_screenshot_get_to_one_related(id, fields_in_app_purchase_app_store_review_screenshots=fields_in_app_purchase_app_store_review_screenshots, fields_in_app_purchases=fields_in_app_purchases, include=include)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_app_store_review_screenshot_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_app_store_review_screenshot_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_in_app_purchase_app_store_review_screenshots** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchaseAppStoreReviewScreenshots | [optional] 
 **fields_in_app_purchases** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchases | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**InAppPurchaseAppStoreReviewScreenshotResponse**](InAppPurchaseAppStoreReviewScreenshotResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Single InAppPurchaseAppStoreReviewScreenshot |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_app_store_review_screenshot_get_to_one_relationship**
> InAppPurchaseV2AppStoreReviewScreenshotLinkageResponse in_app_purchases_v2_app_store_review_screenshot_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_v2_app_store_review_screenshot_linkage_response import InAppPurchaseV2AppStoreReviewScreenshotLinkageResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.in_app_purchases_v2_app_store_review_screenshot_get_to_one_relationship(id)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_app_store_review_screenshot_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_app_store_review_screenshot_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**InAppPurchaseV2AppStoreReviewScreenshotLinkageResponse**](InAppPurchaseV2AppStoreReviewScreenshotLinkageResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Related linkage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_content_get_to_one_related**
> InAppPurchaseContentResponse in_app_purchases_v2_content_get_to_one_related(id, fields_in_app_purchase_contents=fields_in_app_purchase_contents, fields_in_app_purchases=fields_in_app_purchases, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_content_response import InAppPurchaseContentResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_in_app_purchase_contents = ['fields_in_app_purchase_contents_example'] # List[str] | the fields to include for returned resources of type inAppPurchaseContents (optional)
    fields_in_app_purchases = ['fields_in_app_purchases_example'] # List[str] | the fields to include for returned resources of type inAppPurchases (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.in_app_purchases_v2_content_get_to_one_related(id, fields_in_app_purchase_contents=fields_in_app_purchase_contents, fields_in_app_purchases=fields_in_app_purchases, include=include)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_content_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_content_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_in_app_purchase_contents** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchaseContents | [optional] 
 **fields_in_app_purchases** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchases | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**InAppPurchaseContentResponse**](InAppPurchaseContentResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Single InAppPurchaseContent |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_content_get_to_one_relationship**
> InAppPurchaseV2ContentLinkageResponse in_app_purchases_v2_content_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_v2_content_linkage_response import InAppPurchaseV2ContentLinkageResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.in_app_purchases_v2_content_get_to_one_relationship(id)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_content_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_content_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**InAppPurchaseV2ContentLinkageResponse**](InAppPurchaseV2ContentLinkageResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Related linkage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_create_instance**
> InAppPurchaseV2Response in_app_purchases_v2_create_instance(in_app_purchase_v2_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_v2_create_request import InAppPurchaseV2CreateRequest
from openapi_client.models.in_app_purchase_v2_response import InAppPurchaseV2Response
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    in_app_purchase_v2_create_request = openapi_client.InAppPurchaseV2CreateRequest() # InAppPurchaseV2CreateRequest | InAppPurchase representation

    try:
        api_response = api_instance.in_app_purchases_v2_create_instance(in_app_purchase_v2_create_request)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **in_app_purchase_v2_create_request** | [**InAppPurchaseV2CreateRequest**](InAppPurchaseV2CreateRequest.md)| InAppPurchase representation | 

### Return type

[**InAppPurchaseV2Response**](InAppPurchaseV2Response.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**201** | Single InAppPurchase |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_delete_instance**
> in_app_purchases_v2_delete_instance(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.in_app_purchases_v2_delete_instance(id)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_delete_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**409** | Request entity error(s) |  -  |
**204** | Success (no content) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_get_instance**
> InAppPurchaseV2Response in_app_purchases_v2_get_instance(id, fields_in_app_purchases=fields_in_app_purchases, fields_in_app_purchase_localizations=fields_in_app_purchase_localizations, fields_in_app_purchase_price_points=fields_in_app_purchase_price_points, fields_in_app_purchase_contents=fields_in_app_purchase_contents, fields_in_app_purchase_app_store_review_screenshots=fields_in_app_purchase_app_store_review_screenshots, fields_promoted_purchases=fields_promoted_purchases, fields_in_app_purchase_price_schedules=fields_in_app_purchase_price_schedules, fields_in_app_purchase_availabilities=fields_in_app_purchase_availabilities, fields_in_app_purchase_images=fields_in_app_purchase_images, include=include, limit_images=limit_images, limit_in_app_purchase_localizations=limit_in_app_purchase_localizations, limit_price_points=limit_price_points)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_v2_response import InAppPurchaseV2Response
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_in_app_purchases = ['fields_in_app_purchases_example'] # List[str] | the fields to include for returned resources of type inAppPurchases (optional)
    fields_in_app_purchase_localizations = ['fields_in_app_purchase_localizations_example'] # List[str] | the fields to include for returned resources of type inAppPurchaseLocalizations (optional)
    fields_in_app_purchase_price_points = ['fields_in_app_purchase_price_points_example'] # List[str] | the fields to include for returned resources of type inAppPurchasePricePoints (optional)
    fields_in_app_purchase_contents = ['fields_in_app_purchase_contents_example'] # List[str] | the fields to include for returned resources of type inAppPurchaseContents (optional)
    fields_in_app_purchase_app_store_review_screenshots = ['fields_in_app_purchase_app_store_review_screenshots_example'] # List[str] | the fields to include for returned resources of type inAppPurchaseAppStoreReviewScreenshots (optional)
    fields_promoted_purchases = ['fields_promoted_purchases_example'] # List[str] | the fields to include for returned resources of type promotedPurchases (optional)
    fields_in_app_purchase_price_schedules = ['fields_in_app_purchase_price_schedules_example'] # List[str] | the fields to include for returned resources of type inAppPurchasePriceSchedules (optional)
    fields_in_app_purchase_availabilities = ['fields_in_app_purchase_availabilities_example'] # List[str] | the fields to include for returned resources of type inAppPurchaseAvailabilities (optional)
    fields_in_app_purchase_images = ['fields_in_app_purchase_images_example'] # List[str] | the fields to include for returned resources of type inAppPurchaseImages (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_images = 56 # int | maximum number of related images returned (when they are included) (optional)
    limit_in_app_purchase_localizations = 56 # int | maximum number of related inAppPurchaseLocalizations returned (when they are included) (optional)
    limit_price_points = 56 # int | maximum number of related pricePoints returned (when they are included) (optional)

    try:
        api_response = api_instance.in_app_purchases_v2_get_instance(id, fields_in_app_purchases=fields_in_app_purchases, fields_in_app_purchase_localizations=fields_in_app_purchase_localizations, fields_in_app_purchase_price_points=fields_in_app_purchase_price_points, fields_in_app_purchase_contents=fields_in_app_purchase_contents, fields_in_app_purchase_app_store_review_screenshots=fields_in_app_purchase_app_store_review_screenshots, fields_promoted_purchases=fields_promoted_purchases, fields_in_app_purchase_price_schedules=fields_in_app_purchase_price_schedules, fields_in_app_purchase_availabilities=fields_in_app_purchase_availabilities, fields_in_app_purchase_images=fields_in_app_purchase_images, include=include, limit_images=limit_images, limit_in_app_purchase_localizations=limit_in_app_purchase_localizations, limit_price_points=limit_price_points)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_in_app_purchases** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchases | [optional] 
 **fields_in_app_purchase_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchaseLocalizations | [optional] 
 **fields_in_app_purchase_price_points** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchasePricePoints | [optional] 
 **fields_in_app_purchase_contents** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchaseContents | [optional] 
 **fields_in_app_purchase_app_store_review_screenshots** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchaseAppStoreReviewScreenshots | [optional] 
 **fields_promoted_purchases** | [**List[str]**](str.md)| the fields to include for returned resources of type promotedPurchases | [optional] 
 **fields_in_app_purchase_price_schedules** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchasePriceSchedules | [optional] 
 **fields_in_app_purchase_availabilities** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchaseAvailabilities | [optional] 
 **fields_in_app_purchase_images** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchaseImages | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_images** | **int**| maximum number of related images returned (when they are included) | [optional] 
 **limit_in_app_purchase_localizations** | **int**| maximum number of related inAppPurchaseLocalizations returned (when they are included) | [optional] 
 **limit_price_points** | **int**| maximum number of related pricePoints returned (when they are included) | [optional] 

### Return type

[**InAppPurchaseV2Response**](InAppPurchaseV2Response.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Single InAppPurchase |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_iap_price_schedule_get_to_one_related**
> InAppPurchasePriceScheduleResponse in_app_purchases_v2_iap_price_schedule_get_to_one_related(id, fields_in_app_purchase_price_schedules=fields_in_app_purchase_price_schedules, fields_territories=fields_territories, fields_in_app_purchase_prices=fields_in_app_purchase_prices, include=include, limit_manual_prices=limit_manual_prices, limit_automatic_prices=limit_automatic_prices)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_price_schedule_response import InAppPurchasePriceScheduleResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_in_app_purchase_price_schedules = ['fields_in_app_purchase_price_schedules_example'] # List[str] | the fields to include for returned resources of type inAppPurchasePriceSchedules (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    fields_in_app_purchase_prices = ['fields_in_app_purchase_prices_example'] # List[str] | the fields to include for returned resources of type inAppPurchasePrices (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_manual_prices = 56 # int | maximum number of related manualPrices returned (when they are included) (optional)
    limit_automatic_prices = 56 # int | maximum number of related automaticPrices returned (when they are included) (optional)

    try:
        api_response = api_instance.in_app_purchases_v2_iap_price_schedule_get_to_one_related(id, fields_in_app_purchase_price_schedules=fields_in_app_purchase_price_schedules, fields_territories=fields_territories, fields_in_app_purchase_prices=fields_in_app_purchase_prices, include=include, limit_manual_prices=limit_manual_prices, limit_automatic_prices=limit_automatic_prices)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_iap_price_schedule_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_iap_price_schedule_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_in_app_purchase_price_schedules** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchasePriceSchedules | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **fields_in_app_purchase_prices** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchasePrices | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_manual_prices** | **int**| maximum number of related manualPrices returned (when they are included) | [optional] 
 **limit_automatic_prices** | **int**| maximum number of related automaticPrices returned (when they are included) | [optional] 

### Return type

[**InAppPurchasePriceScheduleResponse**](InAppPurchasePriceScheduleResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Single InAppPurchasePriceSchedule |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_iap_price_schedule_get_to_one_relationship**
> InAppPurchaseV2IapPriceScheduleLinkageResponse in_app_purchases_v2_iap_price_schedule_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_v2_iap_price_schedule_linkage_response import InAppPurchaseV2IapPriceScheduleLinkageResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.in_app_purchases_v2_iap_price_schedule_get_to_one_relationship(id)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_iap_price_schedule_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_iap_price_schedule_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**InAppPurchaseV2IapPriceScheduleLinkageResponse**](InAppPurchaseV2IapPriceScheduleLinkageResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Related linkage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_images_get_to_many_related**
> InAppPurchaseImagesResponse in_app_purchases_v2_images_get_to_many_related(id, fields_in_app_purchase_images=fields_in_app_purchase_images, fields_in_app_purchases=fields_in_app_purchases, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_images_response import InAppPurchaseImagesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_in_app_purchase_images = ['fields_in_app_purchase_images_example'] # List[str] | the fields to include for returned resources of type inAppPurchaseImages (optional)
    fields_in_app_purchases = ['fields_in_app_purchases_example'] # List[str] | the fields to include for returned resources of type inAppPurchases (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.in_app_purchases_v2_images_get_to_many_related(id, fields_in_app_purchase_images=fields_in_app_purchase_images, fields_in_app_purchases=fields_in_app_purchases, limit=limit, include=include)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_images_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_images_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_in_app_purchase_images** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchaseImages | [optional] 
 **fields_in_app_purchases** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchases | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**InAppPurchaseImagesResponse**](InAppPurchaseImagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of InAppPurchaseImages |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_images_get_to_many_relationship**
> InAppPurchaseV2ImagesLinkagesResponse in_app_purchases_v2_images_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_v2_images_linkages_response import InAppPurchaseV2ImagesLinkagesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.in_app_purchases_v2_images_get_to_many_relationship(id, limit=limit)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_images_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_images_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**InAppPurchaseV2ImagesLinkagesResponse**](InAppPurchaseV2ImagesLinkagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of related linkages |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_in_app_purchase_availability_get_to_one_related**
> InAppPurchaseAvailabilityResponse in_app_purchases_v2_in_app_purchase_availability_get_to_one_related(id, fields_in_app_purchase_availabilities=fields_in_app_purchase_availabilities, fields_territories=fields_territories, include=include, limit_available_territories=limit_available_territories)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_availability_response import InAppPurchaseAvailabilityResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_in_app_purchase_availabilities = ['fields_in_app_purchase_availabilities_example'] # List[str] | the fields to include for returned resources of type inAppPurchaseAvailabilities (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_available_territories = 56 # int | maximum number of related availableTerritories returned (when they are included) (optional)

    try:
        api_response = api_instance.in_app_purchases_v2_in_app_purchase_availability_get_to_one_related(id, fields_in_app_purchase_availabilities=fields_in_app_purchase_availabilities, fields_territories=fields_territories, include=include, limit_available_territories=limit_available_territories)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_in_app_purchase_availability_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_in_app_purchase_availability_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_in_app_purchase_availabilities** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchaseAvailabilities | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_available_territories** | **int**| maximum number of related availableTerritories returned (when they are included) | [optional] 

### Return type

[**InAppPurchaseAvailabilityResponse**](InAppPurchaseAvailabilityResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Single InAppPurchaseAvailability |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_in_app_purchase_availability_get_to_one_relationship**
> InAppPurchaseV2InAppPurchaseAvailabilityLinkageResponse in_app_purchases_v2_in_app_purchase_availability_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_v2_in_app_purchase_availability_linkage_response import InAppPurchaseV2InAppPurchaseAvailabilityLinkageResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.in_app_purchases_v2_in_app_purchase_availability_get_to_one_relationship(id)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_in_app_purchase_availability_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_in_app_purchase_availability_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**InAppPurchaseV2InAppPurchaseAvailabilityLinkageResponse**](InAppPurchaseV2InAppPurchaseAvailabilityLinkageResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Related linkage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_in_app_purchase_localizations_get_to_many_related**
> InAppPurchaseLocalizationsResponse in_app_purchases_v2_in_app_purchase_localizations_get_to_many_related(id, fields_in_app_purchase_localizations=fields_in_app_purchase_localizations, fields_in_app_purchases=fields_in_app_purchases, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_localizations_response import InAppPurchaseLocalizationsResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_in_app_purchase_localizations = ['fields_in_app_purchase_localizations_example'] # List[str] | the fields to include for returned resources of type inAppPurchaseLocalizations (optional)
    fields_in_app_purchases = ['fields_in_app_purchases_example'] # List[str] | the fields to include for returned resources of type inAppPurchases (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.in_app_purchases_v2_in_app_purchase_localizations_get_to_many_related(id, fields_in_app_purchase_localizations=fields_in_app_purchase_localizations, fields_in_app_purchases=fields_in_app_purchases, limit=limit, include=include)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_in_app_purchase_localizations_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_in_app_purchase_localizations_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_in_app_purchase_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchaseLocalizations | [optional] 
 **fields_in_app_purchases** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchases | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**InAppPurchaseLocalizationsResponse**](InAppPurchaseLocalizationsResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of InAppPurchaseLocalizations |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_in_app_purchase_localizations_get_to_many_relationship**
> InAppPurchaseV2InAppPurchaseLocalizationsLinkagesResponse in_app_purchases_v2_in_app_purchase_localizations_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_v2_in_app_purchase_localizations_linkages_response import InAppPurchaseV2InAppPurchaseLocalizationsLinkagesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.in_app_purchases_v2_in_app_purchase_localizations_get_to_many_relationship(id, limit=limit)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_in_app_purchase_localizations_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_in_app_purchase_localizations_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**InAppPurchaseV2InAppPurchaseLocalizationsLinkagesResponse**](InAppPurchaseV2InAppPurchaseLocalizationsLinkagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of related linkages |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_price_points_get_to_many_related**
> InAppPurchasePricePointsResponse in_app_purchases_v2_price_points_get_to_many_related(id, filter_territory=filter_territory, fields_in_app_purchase_price_points=fields_in_app_purchase_price_points, fields_territories=fields_territories, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_price_points_response import InAppPurchasePricePointsResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_territory = ['filter_territory_example'] # List[str] | filter by id(s) of related 'territory' (optional)
    fields_in_app_purchase_price_points = ['fields_in_app_purchase_price_points_example'] # List[str] | the fields to include for returned resources of type inAppPurchasePricePoints (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.in_app_purchases_v2_price_points_get_to_many_related(id, filter_territory=filter_territory, fields_in_app_purchase_price_points=fields_in_app_purchase_price_points, fields_territories=fields_territories, limit=limit, include=include)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_price_points_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_price_points_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_territory** | [**List[str]**](str.md)| filter by id(s) of related &#39;territory&#39; | [optional] 
 **fields_in_app_purchase_price_points** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchasePricePoints | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**InAppPurchasePricePointsResponse**](InAppPurchasePricePointsResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/csv

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of InAppPurchasePricePoints |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_price_points_get_to_many_relationship**
> InAppPurchaseV2PricePointsLinkagesResponse in_app_purchases_v2_price_points_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_v2_price_points_linkages_response import InAppPurchaseV2PricePointsLinkagesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.in_app_purchases_v2_price_points_get_to_many_relationship(id, limit=limit)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_price_points_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_price_points_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**InAppPurchaseV2PricePointsLinkagesResponse**](InAppPurchaseV2PricePointsLinkagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of related linkages |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_promoted_purchase_get_to_one_related**
> PromotedPurchaseResponse in_app_purchases_v2_promoted_purchase_get_to_one_related(id, fields_promoted_purchases=fields_promoted_purchases, fields_in_app_purchases=fields_in_app_purchases, fields_subscriptions=fields_subscriptions, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.promoted_purchase_response import PromotedPurchaseResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_promoted_purchases = ['fields_promoted_purchases_example'] # List[str] | the fields to include for returned resources of type promotedPurchases (optional)
    fields_in_app_purchases = ['fields_in_app_purchases_example'] # List[str] | the fields to include for returned resources of type inAppPurchases (optional)
    fields_subscriptions = ['fields_subscriptions_example'] # List[str] | the fields to include for returned resources of type subscriptions (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.in_app_purchases_v2_promoted_purchase_get_to_one_related(id, fields_promoted_purchases=fields_promoted_purchases, fields_in_app_purchases=fields_in_app_purchases, fields_subscriptions=fields_subscriptions, include=include)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_promoted_purchase_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_promoted_purchase_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_promoted_purchases** | [**List[str]**](str.md)| the fields to include for returned resources of type promotedPurchases | [optional] 
 **fields_in_app_purchases** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchases | [optional] 
 **fields_subscriptions** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptions | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**PromotedPurchaseResponse**](PromotedPurchaseResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Single PromotedPurchase |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_promoted_purchase_get_to_one_relationship**
> InAppPurchaseV2PromotedPurchaseLinkageResponse in_app_purchases_v2_promoted_purchase_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_v2_promoted_purchase_linkage_response import InAppPurchaseV2PromotedPurchaseLinkageResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.in_app_purchases_v2_promoted_purchase_get_to_one_relationship(id)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_promoted_purchase_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_promoted_purchase_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**InAppPurchaseV2PromotedPurchaseLinkageResponse**](InAppPurchaseV2PromotedPurchaseLinkageResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Related linkage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **in_app_purchases_v2_update_instance**
> InAppPurchaseV2Response in_app_purchases_v2_update_instance(id, in_app_purchase_v2_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.in_app_purchase_v2_response import InAppPurchaseV2Response
from openapi_client.models.in_app_purchase_v2_update_request import InAppPurchaseV2UpdateRequest
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.InAppPurchasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    in_app_purchase_v2_update_request = openapi_client.InAppPurchaseV2UpdateRequest() # InAppPurchaseV2UpdateRequest | InAppPurchase representation

    try:
        api_response = api_instance.in_app_purchases_v2_update_instance(id, in_app_purchase_v2_update_request)
        print("The response of InAppPurchasesApi->in_app_purchases_v2_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InAppPurchasesApi->in_app_purchases_v2_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **in_app_purchase_v2_update_request** | [**InAppPurchaseV2UpdateRequest**](InAppPurchaseV2UpdateRequest.md)| InAppPurchase representation | 

### Return type

[**InAppPurchaseV2Response**](InAppPurchaseV2Response.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**200** | Single InAppPurchase |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

