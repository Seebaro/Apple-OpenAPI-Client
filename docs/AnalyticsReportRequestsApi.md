# openapi_client.AnalyticsReportRequestsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**analytics_report_requests_create_instance**](AnalyticsReportRequestsApi.md#analytics_report_requests_create_instance) | **POST** /v1/analyticsReportRequests | 
[**analytics_report_requests_delete_instance**](AnalyticsReportRequestsApi.md#analytics_report_requests_delete_instance) | **DELETE** /v1/analyticsReportRequests/{id} | 
[**analytics_report_requests_get_instance**](AnalyticsReportRequestsApi.md#analytics_report_requests_get_instance) | **GET** /v1/analyticsReportRequests/{id} | 
[**analytics_report_requests_reports_get_to_many_related**](AnalyticsReportRequestsApi.md#analytics_report_requests_reports_get_to_many_related) | **GET** /v1/analyticsReportRequests/{id}/reports | 
[**analytics_report_requests_reports_get_to_many_relationship**](AnalyticsReportRequestsApi.md#analytics_report_requests_reports_get_to_many_relationship) | **GET** /v1/analyticsReportRequests/{id}/relationships/reports | 


# **analytics_report_requests_create_instance**
> AnalyticsReportRequestResponse analytics_report_requests_create_instance(analytics_report_request_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.analytics_report_request_create_request import AnalyticsReportRequestCreateRequest
from openapi_client.models.analytics_report_request_response import AnalyticsReportRequestResponse
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
    api_instance = openapi_client.AnalyticsReportRequestsApi(api_client)
    analytics_report_request_create_request = openapi_client.AnalyticsReportRequestCreateRequest() # AnalyticsReportRequestCreateRequest | AnalyticsReportRequest representation

    try:
        api_response = api_instance.analytics_report_requests_create_instance(analytics_report_request_create_request)
        print("The response of AnalyticsReportRequestsApi->analytics_report_requests_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyticsReportRequestsApi->analytics_report_requests_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **analytics_report_request_create_request** | [**AnalyticsReportRequestCreateRequest**](AnalyticsReportRequestCreateRequest.md)| AnalyticsReportRequest representation | 

### Return type

[**AnalyticsReportRequestResponse**](AnalyticsReportRequestResponse.md)

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
**201** | Single AnalyticsReportRequest |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analytics_report_requests_delete_instance**
> analytics_report_requests_delete_instance(id)

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
    api_instance = openapi_client.AnalyticsReportRequestsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.analytics_report_requests_delete_instance(id)
    except Exception as e:
        print("Exception when calling AnalyticsReportRequestsApi->analytics_report_requests_delete_instance: %s\n" % e)
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

# **analytics_report_requests_get_instance**
> AnalyticsReportRequestResponse analytics_report_requests_get_instance(id, fields_analytics_report_requests=fields_analytics_report_requests, fields_analytics_reports=fields_analytics_reports, include=include, limit_reports=limit_reports)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.analytics_report_request_response import AnalyticsReportRequestResponse
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
    api_instance = openapi_client.AnalyticsReportRequestsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_analytics_report_requests = ['fields_analytics_report_requests_example'] # List[str] | the fields to include for returned resources of type analyticsReportRequests (optional)
    fields_analytics_reports = ['fields_analytics_reports_example'] # List[str] | the fields to include for returned resources of type analyticsReports (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_reports = 56 # int | maximum number of related reports returned (when they are included) (optional)

    try:
        api_response = api_instance.analytics_report_requests_get_instance(id, fields_analytics_report_requests=fields_analytics_report_requests, fields_analytics_reports=fields_analytics_reports, include=include, limit_reports=limit_reports)
        print("The response of AnalyticsReportRequestsApi->analytics_report_requests_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyticsReportRequestsApi->analytics_report_requests_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_analytics_report_requests** | [**List[str]**](str.md)| the fields to include for returned resources of type analyticsReportRequests | [optional] 
 **fields_analytics_reports** | [**List[str]**](str.md)| the fields to include for returned resources of type analyticsReports | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_reports** | **int**| maximum number of related reports returned (when they are included) | [optional] 

### Return type

[**AnalyticsReportRequestResponse**](AnalyticsReportRequestResponse.md)

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
**200** | Single AnalyticsReportRequest |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analytics_report_requests_reports_get_to_many_related**
> AnalyticsReportsResponse analytics_report_requests_reports_get_to_many_related(id, filter_name=filter_name, filter_category=filter_category, fields_analytics_reports=fields_analytics_reports, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.analytics_reports_response import AnalyticsReportsResponse
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
    api_instance = openapi_client.AnalyticsReportRequestsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_name = ['filter_name_example'] # List[str] | filter by attribute 'name' (optional)
    filter_category = ['filter_category_example'] # List[str] | filter by attribute 'category' (optional)
    fields_analytics_reports = ['fields_analytics_reports_example'] # List[str] | the fields to include for returned resources of type analyticsReports (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.analytics_report_requests_reports_get_to_many_related(id, filter_name=filter_name, filter_category=filter_category, fields_analytics_reports=fields_analytics_reports, limit=limit)
        print("The response of AnalyticsReportRequestsApi->analytics_report_requests_reports_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyticsReportRequestsApi->analytics_report_requests_reports_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_name** | [**List[str]**](str.md)| filter by attribute &#39;name&#39; | [optional] 
 **filter_category** | [**List[str]**](str.md)| filter by attribute &#39;category&#39; | [optional] 
 **fields_analytics_reports** | [**List[str]**](str.md)| the fields to include for returned resources of type analyticsReports | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AnalyticsReportsResponse**](AnalyticsReportsResponse.md)

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
**200** | List of AnalyticsReports |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analytics_report_requests_reports_get_to_many_relationship**
> AnalyticsReportRequestReportsLinkagesResponse analytics_report_requests_reports_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.analytics_report_request_reports_linkages_response import AnalyticsReportRequestReportsLinkagesResponse
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
    api_instance = openapi_client.AnalyticsReportRequestsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.analytics_report_requests_reports_get_to_many_relationship(id, limit=limit)
        print("The response of AnalyticsReportRequestsApi->analytics_report_requests_reports_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyticsReportRequestsApi->analytics_report_requests_reports_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AnalyticsReportRequestReportsLinkagesResponse**](AnalyticsReportRequestReportsLinkagesResponse.md)

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

