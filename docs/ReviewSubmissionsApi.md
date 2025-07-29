# openapi_client.ReviewSubmissionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**review_submissions_create_instance**](ReviewSubmissionsApi.md#review_submissions_create_instance) | **POST** /v1/reviewSubmissions | 
[**review_submissions_get_collection**](ReviewSubmissionsApi.md#review_submissions_get_collection) | **GET** /v1/reviewSubmissions | 
[**review_submissions_get_instance**](ReviewSubmissionsApi.md#review_submissions_get_instance) | **GET** /v1/reviewSubmissions/{id} | 
[**review_submissions_items_get_to_many_related**](ReviewSubmissionsApi.md#review_submissions_items_get_to_many_related) | **GET** /v1/reviewSubmissions/{id}/items | 
[**review_submissions_items_get_to_many_relationship**](ReviewSubmissionsApi.md#review_submissions_items_get_to_many_relationship) | **GET** /v1/reviewSubmissions/{id}/relationships/items | 
[**review_submissions_update_instance**](ReviewSubmissionsApi.md#review_submissions_update_instance) | **PATCH** /v1/reviewSubmissions/{id} | 


# **review_submissions_create_instance**
> ReviewSubmissionResponse review_submissions_create_instance(review_submission_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.review_submission_create_request import ReviewSubmissionCreateRequest
from openapi_client.models.review_submission_response import ReviewSubmissionResponse
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
    api_instance = openapi_client.ReviewSubmissionsApi(api_client)
    review_submission_create_request = openapi_client.ReviewSubmissionCreateRequest() # ReviewSubmissionCreateRequest | ReviewSubmission representation

    try:
        api_response = api_instance.review_submissions_create_instance(review_submission_create_request)
        print("The response of ReviewSubmissionsApi->review_submissions_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReviewSubmissionsApi->review_submissions_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **review_submission_create_request** | [**ReviewSubmissionCreateRequest**](ReviewSubmissionCreateRequest.md)| ReviewSubmission representation | 

### Return type

[**ReviewSubmissionResponse**](ReviewSubmissionResponse.md)

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
**201** | Single ReviewSubmission |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **review_submissions_get_collection**
> ReviewSubmissionsResponse review_submissions_get_collection(filter_app, filter_platform=filter_platform, filter_state=filter_state, fields_review_submissions=fields_review_submissions, fields_review_submission_items=fields_review_submission_items, limit=limit, include=include, limit_items=limit_items)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.review_submissions_response import ReviewSubmissionsResponse
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
    api_instance = openapi_client.ReviewSubmissionsApi(api_client)
    filter_app = ['filter_app_example'] # List[str] | filter by id(s) of related 'app'
    filter_platform = ['filter_platform_example'] # List[str] | filter by attribute 'platform' (optional)
    filter_state = ['filter_state_example'] # List[str] | filter by attribute 'state' (optional)
    fields_review_submissions = ['fields_review_submissions_example'] # List[str] | the fields to include for returned resources of type reviewSubmissions (optional)
    fields_review_submission_items = ['fields_review_submission_items_example'] # List[str] | the fields to include for returned resources of type reviewSubmissionItems (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_items = 56 # int | maximum number of related items returned (when they are included) (optional)

    try:
        api_response = api_instance.review_submissions_get_collection(filter_app, filter_platform=filter_platform, filter_state=filter_state, fields_review_submissions=fields_review_submissions, fields_review_submission_items=fields_review_submission_items, limit=limit, include=include, limit_items=limit_items)
        print("The response of ReviewSubmissionsApi->review_submissions_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReviewSubmissionsApi->review_submissions_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter_app** | [**List[str]**](str.md)| filter by id(s) of related &#39;app&#39; | 
 **filter_platform** | [**List[str]**](str.md)| filter by attribute &#39;platform&#39; | [optional] 
 **filter_state** | [**List[str]**](str.md)| filter by attribute &#39;state&#39; | [optional] 
 **fields_review_submissions** | [**List[str]**](str.md)| the fields to include for returned resources of type reviewSubmissions | [optional] 
 **fields_review_submission_items** | [**List[str]**](str.md)| the fields to include for returned resources of type reviewSubmissionItems | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_items** | **int**| maximum number of related items returned (when they are included) | [optional] 

### Return type

[**ReviewSubmissionsResponse**](ReviewSubmissionsResponse.md)

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
**200** | List of ReviewSubmissions |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **review_submissions_get_instance**
> ReviewSubmissionResponse review_submissions_get_instance(id, fields_review_submissions=fields_review_submissions, fields_review_submission_items=fields_review_submission_items, include=include, limit_items=limit_items)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.review_submission_response import ReviewSubmissionResponse
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
    api_instance = openapi_client.ReviewSubmissionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_review_submissions = ['fields_review_submissions_example'] # List[str] | the fields to include for returned resources of type reviewSubmissions (optional)
    fields_review_submission_items = ['fields_review_submission_items_example'] # List[str] | the fields to include for returned resources of type reviewSubmissionItems (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_items = 56 # int | maximum number of related items returned (when they are included) (optional)

    try:
        api_response = api_instance.review_submissions_get_instance(id, fields_review_submissions=fields_review_submissions, fields_review_submission_items=fields_review_submission_items, include=include, limit_items=limit_items)
        print("The response of ReviewSubmissionsApi->review_submissions_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReviewSubmissionsApi->review_submissions_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_review_submissions** | [**List[str]**](str.md)| the fields to include for returned resources of type reviewSubmissions | [optional] 
 **fields_review_submission_items** | [**List[str]**](str.md)| the fields to include for returned resources of type reviewSubmissionItems | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_items** | **int**| maximum number of related items returned (when they are included) | [optional] 

### Return type

[**ReviewSubmissionResponse**](ReviewSubmissionResponse.md)

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
**200** | Single ReviewSubmission |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **review_submissions_items_get_to_many_related**
> ReviewSubmissionItemsResponse review_submissions_items_get_to_many_related(id, fields_review_submission_items=fields_review_submission_items, fields_app_store_versions=fields_app_store_versions, fields_app_custom_product_page_versions=fields_app_custom_product_page_versions, fields_app_store_version_experiments=fields_app_store_version_experiments, fields_app_events=fields_app_events, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.review_submission_items_response import ReviewSubmissionItemsResponse
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
    api_instance = openapi_client.ReviewSubmissionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_review_submission_items = ['fields_review_submission_items_example'] # List[str] | the fields to include for returned resources of type reviewSubmissionItems (optional)
    fields_app_store_versions = ['fields_app_store_versions_example'] # List[str] | the fields to include for returned resources of type appStoreVersions (optional)
    fields_app_custom_product_page_versions = ['fields_app_custom_product_page_versions_example'] # List[str] | the fields to include for returned resources of type appCustomProductPageVersions (optional)
    fields_app_store_version_experiments = ['fields_app_store_version_experiments_example'] # List[str] | the fields to include for returned resources of type appStoreVersionExperiments (optional)
    fields_app_events = ['fields_app_events_example'] # List[str] | the fields to include for returned resources of type appEvents (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.review_submissions_items_get_to_many_related(id, fields_review_submission_items=fields_review_submission_items, fields_app_store_versions=fields_app_store_versions, fields_app_custom_product_page_versions=fields_app_custom_product_page_versions, fields_app_store_version_experiments=fields_app_store_version_experiments, fields_app_events=fields_app_events, limit=limit, include=include)
        print("The response of ReviewSubmissionsApi->review_submissions_items_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReviewSubmissionsApi->review_submissions_items_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_review_submission_items** | [**List[str]**](str.md)| the fields to include for returned resources of type reviewSubmissionItems | [optional] 
 **fields_app_store_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersions | [optional] 
 **fields_app_custom_product_page_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type appCustomProductPageVersions | [optional] 
 **fields_app_store_version_experiments** | [**List[str]**](str.md)| the fields to include for returned resources of type appStoreVersionExperiments | [optional] 
 **fields_app_events** | [**List[str]**](str.md)| the fields to include for returned resources of type appEvents | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**ReviewSubmissionItemsResponse**](ReviewSubmissionItemsResponse.md)

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
**200** | List of ReviewSubmissionItems |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **review_submissions_items_get_to_many_relationship**
> ReviewSubmissionItemsLinkagesResponse review_submissions_items_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.review_submission_items_linkages_response import ReviewSubmissionItemsLinkagesResponse
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
    api_instance = openapi_client.ReviewSubmissionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.review_submissions_items_get_to_many_relationship(id, limit=limit)
        print("The response of ReviewSubmissionsApi->review_submissions_items_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReviewSubmissionsApi->review_submissions_items_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**ReviewSubmissionItemsLinkagesResponse**](ReviewSubmissionItemsLinkagesResponse.md)

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

# **review_submissions_update_instance**
> ReviewSubmissionResponse review_submissions_update_instance(id, review_submission_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.review_submission_response import ReviewSubmissionResponse
from openapi_client.models.review_submission_update_request import ReviewSubmissionUpdateRequest
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
    api_instance = openapi_client.ReviewSubmissionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    review_submission_update_request = openapi_client.ReviewSubmissionUpdateRequest() # ReviewSubmissionUpdateRequest | ReviewSubmission representation

    try:
        api_response = api_instance.review_submissions_update_instance(id, review_submission_update_request)
        print("The response of ReviewSubmissionsApi->review_submissions_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReviewSubmissionsApi->review_submissions_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **review_submission_update_request** | [**ReviewSubmissionUpdateRequest**](ReviewSubmissionUpdateRequest.md)| ReviewSubmission representation | 

### Return type

[**ReviewSubmissionResponse**](ReviewSubmissionResponse.md)

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
**200** | Single ReviewSubmission |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

