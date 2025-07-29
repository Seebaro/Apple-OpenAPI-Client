# openapi_client.BetaFeedbackCrashSubmissionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**beta_feedback_crash_submissions_crash_log_get_to_one_related**](BetaFeedbackCrashSubmissionsApi.md#beta_feedback_crash_submissions_crash_log_get_to_one_related) | **GET** /v1/betaFeedbackCrashSubmissions/{id}/crashLog | 
[**beta_feedback_crash_submissions_crash_log_get_to_one_relationship**](BetaFeedbackCrashSubmissionsApi.md#beta_feedback_crash_submissions_crash_log_get_to_one_relationship) | **GET** /v1/betaFeedbackCrashSubmissions/{id}/relationships/crashLog | 
[**beta_feedback_crash_submissions_delete_instance**](BetaFeedbackCrashSubmissionsApi.md#beta_feedback_crash_submissions_delete_instance) | **DELETE** /v1/betaFeedbackCrashSubmissions/{id} | 
[**beta_feedback_crash_submissions_get_instance**](BetaFeedbackCrashSubmissionsApi.md#beta_feedback_crash_submissions_get_instance) | **GET** /v1/betaFeedbackCrashSubmissions/{id} | 


# **beta_feedback_crash_submissions_crash_log_get_to_one_related**
> BetaCrashLogResponse beta_feedback_crash_submissions_crash_log_get_to_one_related(id, fields_beta_crash_logs=fields_beta_crash_logs)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_crash_log_response import BetaCrashLogResponse
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
    api_instance = openapi_client.BetaFeedbackCrashSubmissionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_beta_crash_logs = ['fields_beta_crash_logs_example'] # List[str] | the fields to include for returned resources of type betaCrashLogs (optional)

    try:
        api_response = api_instance.beta_feedback_crash_submissions_crash_log_get_to_one_related(id, fields_beta_crash_logs=fields_beta_crash_logs)
        print("The response of BetaFeedbackCrashSubmissionsApi->beta_feedback_crash_submissions_crash_log_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BetaFeedbackCrashSubmissionsApi->beta_feedback_crash_submissions_crash_log_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_beta_crash_logs** | [**List[str]**](str.md)| the fields to include for returned resources of type betaCrashLogs | [optional] 

### Return type

[**BetaCrashLogResponse**](BetaCrashLogResponse.md)

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
**200** | Single BetaCrashLog |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **beta_feedback_crash_submissions_crash_log_get_to_one_relationship**
> BetaFeedbackCrashSubmissionCrashLogLinkageResponse beta_feedback_crash_submissions_crash_log_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_feedback_crash_submission_crash_log_linkage_response import BetaFeedbackCrashSubmissionCrashLogLinkageResponse
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
    api_instance = openapi_client.BetaFeedbackCrashSubmissionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.beta_feedback_crash_submissions_crash_log_get_to_one_relationship(id)
        print("The response of BetaFeedbackCrashSubmissionsApi->beta_feedback_crash_submissions_crash_log_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BetaFeedbackCrashSubmissionsApi->beta_feedback_crash_submissions_crash_log_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**BetaFeedbackCrashSubmissionCrashLogLinkageResponse**](BetaFeedbackCrashSubmissionCrashLogLinkageResponse.md)

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

# **beta_feedback_crash_submissions_delete_instance**
> beta_feedback_crash_submissions_delete_instance(id)

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
    api_instance = openapi_client.BetaFeedbackCrashSubmissionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.beta_feedback_crash_submissions_delete_instance(id)
    except Exception as e:
        print("Exception when calling BetaFeedbackCrashSubmissionsApi->beta_feedback_crash_submissions_delete_instance: %s\n" % e)
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

# **beta_feedback_crash_submissions_get_instance**
> BetaFeedbackCrashSubmissionResponse beta_feedback_crash_submissions_get_instance(id, fields_beta_feedback_crash_submissions=fields_beta_feedback_crash_submissions, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_feedback_crash_submission_response import BetaFeedbackCrashSubmissionResponse
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
    api_instance = openapi_client.BetaFeedbackCrashSubmissionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_beta_feedback_crash_submissions = ['fields_beta_feedback_crash_submissions_example'] # List[str] | the fields to include for returned resources of type betaFeedbackCrashSubmissions (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.beta_feedback_crash_submissions_get_instance(id, fields_beta_feedback_crash_submissions=fields_beta_feedback_crash_submissions, include=include)
        print("The response of BetaFeedbackCrashSubmissionsApi->beta_feedback_crash_submissions_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BetaFeedbackCrashSubmissionsApi->beta_feedback_crash_submissions_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_beta_feedback_crash_submissions** | [**List[str]**](str.md)| the fields to include for returned resources of type betaFeedbackCrashSubmissions | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**BetaFeedbackCrashSubmissionResponse**](BetaFeedbackCrashSubmissionResponse.md)

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
**200** | Single BetaFeedbackCrashSubmission |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

