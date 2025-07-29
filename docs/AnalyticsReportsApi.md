# openapi_client.AnalyticsReportsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**analytics_reports_get_instance**](AnalyticsReportsApi.md#analytics_reports_get_instance) | **GET** /v1/analyticsReports/{id} | 
[**analytics_reports_instances_get_to_many_related**](AnalyticsReportsApi.md#analytics_reports_instances_get_to_many_related) | **GET** /v1/analyticsReports/{id}/instances | 
[**analytics_reports_instances_get_to_many_relationship**](AnalyticsReportsApi.md#analytics_reports_instances_get_to_many_relationship) | **GET** /v1/analyticsReports/{id}/relationships/instances | 


# **analytics_reports_get_instance**
> AnalyticsReportResponse analytics_reports_get_instance(id, fields_analytics_reports=fields_analytics_reports)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.analytics_report_response import AnalyticsReportResponse
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
    api_instance = openapi_client.AnalyticsReportsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_analytics_reports = ['fields_analytics_reports_example'] # List[str] | the fields to include for returned resources of type analyticsReports (optional)

    try:
        api_response = api_instance.analytics_reports_get_instance(id, fields_analytics_reports=fields_analytics_reports)
        print("The response of AnalyticsReportsApi->analytics_reports_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyticsReportsApi->analytics_reports_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_analytics_reports** | [**List[str]**](str.md)| the fields to include for returned resources of type analyticsReports | [optional] 

### Return type

[**AnalyticsReportResponse**](AnalyticsReportResponse.md)

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
**200** | Single AnalyticsReport |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analytics_reports_instances_get_to_many_related**
> AnalyticsReportInstancesResponse analytics_reports_instances_get_to_many_related(id, filter_granularity=filter_granularity, filter_processing_date=filter_processing_date, fields_analytics_report_instances=fields_analytics_report_instances, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.analytics_report_instances_response import AnalyticsReportInstancesResponse
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
    api_instance = openapi_client.AnalyticsReportsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_granularity = ['filter_granularity_example'] # List[str] | filter by attribute 'granularity' (optional)
    filter_processing_date = ['filter_processing_date_example'] # List[str] | filter by attribute 'processingDate' (optional)
    fields_analytics_report_instances = ['fields_analytics_report_instances_example'] # List[str] | the fields to include for returned resources of type analyticsReportInstances (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.analytics_reports_instances_get_to_many_related(id, filter_granularity=filter_granularity, filter_processing_date=filter_processing_date, fields_analytics_report_instances=fields_analytics_report_instances, limit=limit)
        print("The response of AnalyticsReportsApi->analytics_reports_instances_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyticsReportsApi->analytics_reports_instances_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_granularity** | [**List[str]**](str.md)| filter by attribute &#39;granularity&#39; | [optional] 
 **filter_processing_date** | [**List[str]**](str.md)| filter by attribute &#39;processingDate&#39; | [optional] 
 **fields_analytics_report_instances** | [**List[str]**](str.md)| the fields to include for returned resources of type analyticsReportInstances | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AnalyticsReportInstancesResponse**](AnalyticsReportInstancesResponse.md)

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
**200** | List of AnalyticsReportInstances |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **analytics_reports_instances_get_to_many_relationship**
> AnalyticsReportInstancesLinkagesResponse analytics_reports_instances_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.analytics_report_instances_linkages_response import AnalyticsReportInstancesLinkagesResponse
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
    api_instance = openapi_client.AnalyticsReportsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.analytics_reports_instances_get_to_many_relationship(id, limit=limit)
        print("The response of AnalyticsReportsApi->analytics_reports_instances_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyticsReportsApi->analytics_reports_instances_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AnalyticsReportInstancesLinkagesResponse**](AnalyticsReportInstancesLinkagesResponse.md)

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

