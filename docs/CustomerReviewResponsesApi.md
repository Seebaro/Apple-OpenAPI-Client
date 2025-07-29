# openapi_client.CustomerReviewResponsesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**customer_review_responses_create_instance**](CustomerReviewResponsesApi.md#customer_review_responses_create_instance) | **POST** /v1/customerReviewResponses | 
[**customer_review_responses_delete_instance**](CustomerReviewResponsesApi.md#customer_review_responses_delete_instance) | **DELETE** /v1/customerReviewResponses/{id} | 
[**customer_review_responses_get_instance**](CustomerReviewResponsesApi.md#customer_review_responses_get_instance) | **GET** /v1/customerReviewResponses/{id} | 


# **customer_review_responses_create_instance**
> CustomerReviewResponseV1Response customer_review_responses_create_instance(customer_review_response_v1_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.customer_review_response_v1_create_request import CustomerReviewResponseV1CreateRequest
from openapi_client.models.customer_review_response_v1_response import CustomerReviewResponseV1Response
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
    api_instance = openapi_client.CustomerReviewResponsesApi(api_client)
    customer_review_response_v1_create_request = openapi_client.CustomerReviewResponseV1CreateRequest() # CustomerReviewResponseV1CreateRequest | CustomerReviewResponse representation

    try:
        api_response = api_instance.customer_review_responses_create_instance(customer_review_response_v1_create_request)
        print("The response of CustomerReviewResponsesApi->customer_review_responses_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerReviewResponsesApi->customer_review_responses_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_review_response_v1_create_request** | [**CustomerReviewResponseV1CreateRequest**](CustomerReviewResponseV1CreateRequest.md)| CustomerReviewResponse representation | 

### Return type

[**CustomerReviewResponseV1Response**](CustomerReviewResponseV1Response.md)

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
**201** | Single CustomerReviewResponse |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **customer_review_responses_delete_instance**
> customer_review_responses_delete_instance(id)

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
    api_instance = openapi_client.CustomerReviewResponsesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.customer_review_responses_delete_instance(id)
    except Exception as e:
        print("Exception when calling CustomerReviewResponsesApi->customer_review_responses_delete_instance: %s\n" % e)
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

# **customer_review_responses_get_instance**
> CustomerReviewResponseV1Response customer_review_responses_get_instance(id, fields_customer_review_responses=fields_customer_review_responses, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.customer_review_response_v1_response import CustomerReviewResponseV1Response
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
    api_instance = openapi_client.CustomerReviewResponsesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_customer_review_responses = ['fields_customer_review_responses_example'] # List[str] | the fields to include for returned resources of type customerReviewResponses (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.customer_review_responses_get_instance(id, fields_customer_review_responses=fields_customer_review_responses, include=include)
        print("The response of CustomerReviewResponsesApi->customer_review_responses_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerReviewResponsesApi->customer_review_responses_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_customer_review_responses** | [**List[str]**](str.md)| the fields to include for returned resources of type customerReviewResponses | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**CustomerReviewResponseV1Response**](CustomerReviewResponseV1Response.md)

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
**200** | Single CustomerReviewResponse |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

