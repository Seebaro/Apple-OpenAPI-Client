# openapi_client.AlternativeDistributionDomainsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**alternative_distribution_domains_create_instance**](AlternativeDistributionDomainsApi.md#alternative_distribution_domains_create_instance) | **POST** /v1/alternativeDistributionDomains | 
[**alternative_distribution_domains_delete_instance**](AlternativeDistributionDomainsApi.md#alternative_distribution_domains_delete_instance) | **DELETE** /v1/alternativeDistributionDomains/{id} | 
[**alternative_distribution_domains_get_collection**](AlternativeDistributionDomainsApi.md#alternative_distribution_domains_get_collection) | **GET** /v1/alternativeDistributionDomains | 
[**alternative_distribution_domains_get_instance**](AlternativeDistributionDomainsApi.md#alternative_distribution_domains_get_instance) | **GET** /v1/alternativeDistributionDomains/{id} | 


# **alternative_distribution_domains_create_instance**
> AlternativeDistributionDomainResponse alternative_distribution_domains_create_instance(alternative_distribution_domain_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.alternative_distribution_domain_create_request import AlternativeDistributionDomainCreateRequest
from openapi_client.models.alternative_distribution_domain_response import AlternativeDistributionDomainResponse
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
    api_instance = openapi_client.AlternativeDistributionDomainsApi(api_client)
    alternative_distribution_domain_create_request = openapi_client.AlternativeDistributionDomainCreateRequest() # AlternativeDistributionDomainCreateRequest | AlternativeDistributionDomain representation

    try:
        api_response = api_instance.alternative_distribution_domains_create_instance(alternative_distribution_domain_create_request)
        print("The response of AlternativeDistributionDomainsApi->alternative_distribution_domains_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlternativeDistributionDomainsApi->alternative_distribution_domains_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **alternative_distribution_domain_create_request** | [**AlternativeDistributionDomainCreateRequest**](AlternativeDistributionDomainCreateRequest.md)| AlternativeDistributionDomain representation | 

### Return type

[**AlternativeDistributionDomainResponse**](AlternativeDistributionDomainResponse.md)

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
**201** | Single AlternativeDistributionDomain |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **alternative_distribution_domains_delete_instance**
> alternative_distribution_domains_delete_instance(id)

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
    api_instance = openapi_client.AlternativeDistributionDomainsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.alternative_distribution_domains_delete_instance(id)
    except Exception as e:
        print("Exception when calling AlternativeDistributionDomainsApi->alternative_distribution_domains_delete_instance: %s\n" % e)
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

# **alternative_distribution_domains_get_collection**
> AlternativeDistributionDomainsResponse alternative_distribution_domains_get_collection(fields_alternative_distribution_domains=fields_alternative_distribution_domains, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.alternative_distribution_domains_response import AlternativeDistributionDomainsResponse
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
    api_instance = openapi_client.AlternativeDistributionDomainsApi(api_client)
    fields_alternative_distribution_domains = ['fields_alternative_distribution_domains_example'] # List[str] | the fields to include for returned resources of type alternativeDistributionDomains (optional)
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.alternative_distribution_domains_get_collection(fields_alternative_distribution_domains=fields_alternative_distribution_domains, limit=limit)
        print("The response of AlternativeDistributionDomainsApi->alternative_distribution_domains_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlternativeDistributionDomainsApi->alternative_distribution_domains_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields_alternative_distribution_domains** | [**List[str]**](str.md)| the fields to include for returned resources of type alternativeDistributionDomains | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**AlternativeDistributionDomainsResponse**](AlternativeDistributionDomainsResponse.md)

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
**200** | List of AlternativeDistributionDomains |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **alternative_distribution_domains_get_instance**
> AlternativeDistributionDomainResponse alternative_distribution_domains_get_instance(id, fields_alternative_distribution_domains=fields_alternative_distribution_domains)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.alternative_distribution_domain_response import AlternativeDistributionDomainResponse
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
    api_instance = openapi_client.AlternativeDistributionDomainsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_alternative_distribution_domains = ['fields_alternative_distribution_domains_example'] # List[str] | the fields to include for returned resources of type alternativeDistributionDomains (optional)

    try:
        api_response = api_instance.alternative_distribution_domains_get_instance(id, fields_alternative_distribution_domains=fields_alternative_distribution_domains)
        print("The response of AlternativeDistributionDomainsApi->alternative_distribution_domains_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AlternativeDistributionDomainsApi->alternative_distribution_domains_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_alternative_distribution_domains** | [**List[str]**](str.md)| the fields to include for returned resources of type alternativeDistributionDomains | [optional] 

### Return type

[**AlternativeDistributionDomainResponse**](AlternativeDistributionDomainResponse.md)

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
**200** | Single AlternativeDistributionDomain |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

