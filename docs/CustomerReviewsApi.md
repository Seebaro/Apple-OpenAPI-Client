# openapi_client.CustomerReviewsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**customer_reviews_get_instance**](CustomerReviewsApi.md#customer_reviews_get_instance) | **GET** /v1/customerReviews/{id} | 
[**customer_reviews_response_get_to_one_related**](CustomerReviewsApi.md#customer_reviews_response_get_to_one_related) | **GET** /v1/customerReviews/{id}/response | 
[**customer_reviews_response_get_to_one_relationship**](CustomerReviewsApi.md#customer_reviews_response_get_to_one_relationship) | **GET** /v1/customerReviews/{id}/relationships/response | 


# **customer_reviews_get_instance**
> CustomerReviewResponse customer_reviews_get_instance(id, fields_customer_reviews=fields_customer_reviews, fields_customer_review_responses=fields_customer_review_responses, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.customer_review_response import CustomerReviewResponse
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
    api_instance = openapi_client.CustomerReviewsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_customer_reviews = ['fields_customer_reviews_example'] # List[str] | the fields to include for returned resources of type customerReviews (optional)
    fields_customer_review_responses = ['fields_customer_review_responses_example'] # List[str] | the fields to include for returned resources of type customerReviewResponses (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.customer_reviews_get_instance(id, fields_customer_reviews=fields_customer_reviews, fields_customer_review_responses=fields_customer_review_responses, include=include)
        print("The response of CustomerReviewsApi->customer_reviews_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerReviewsApi->customer_reviews_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_customer_reviews** | [**List[str]**](str.md)| the fields to include for returned resources of type customerReviews | [optional] 
 **fields_customer_review_responses** | [**List[str]**](str.md)| the fields to include for returned resources of type customerReviewResponses | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**CustomerReviewResponse**](CustomerReviewResponse.md)

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
**200** | Single CustomerReview |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **customer_reviews_response_get_to_one_related**
> CustomerReviewResponseV1Response customer_reviews_response_get_to_one_related(id, fields_customer_review_responses=fields_customer_review_responses, fields_customer_reviews=fields_customer_reviews, include=include)

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
    api_instance = openapi_client.CustomerReviewsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_customer_review_responses = ['fields_customer_review_responses_example'] # List[str] | the fields to include for returned resources of type customerReviewResponses (optional)
    fields_customer_reviews = ['fields_customer_reviews_example'] # List[str] | the fields to include for returned resources of type customerReviews (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.customer_reviews_response_get_to_one_related(id, fields_customer_review_responses=fields_customer_review_responses, fields_customer_reviews=fields_customer_reviews, include=include)
        print("The response of CustomerReviewsApi->customer_reviews_response_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerReviewsApi->customer_reviews_response_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_customer_review_responses** | [**List[str]**](str.md)| the fields to include for returned resources of type customerReviewResponses | [optional] 
 **fields_customer_reviews** | [**List[str]**](str.md)| the fields to include for returned resources of type customerReviews | [optional] 
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

# **customer_reviews_response_get_to_one_relationship**
> CustomerReviewResponseLinkageResponse customer_reviews_response_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.customer_review_response_linkage_response import CustomerReviewResponseLinkageResponse
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
    api_instance = openapi_client.CustomerReviewsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.customer_reviews_response_get_to_one_relationship(id)
        print("The response of CustomerReviewsApi->customer_reviews_response_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerReviewsApi->customer_reviews_response_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**CustomerReviewResponseLinkageResponse**](CustomerReviewResponseLinkageResponse.md)

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

