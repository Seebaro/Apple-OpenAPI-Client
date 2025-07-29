# openapi_client.MerchantIdsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**merchant_ids_certificates_get_to_many_related**](MerchantIdsApi.md#merchant_ids_certificates_get_to_many_related) | **GET** /v1/merchantIds/{id}/certificates | 
[**merchant_ids_certificates_get_to_many_relationship**](MerchantIdsApi.md#merchant_ids_certificates_get_to_many_relationship) | **GET** /v1/merchantIds/{id}/relationships/certificates | 
[**merchant_ids_create_instance**](MerchantIdsApi.md#merchant_ids_create_instance) | **POST** /v1/merchantIds | 
[**merchant_ids_delete_instance**](MerchantIdsApi.md#merchant_ids_delete_instance) | **DELETE** /v1/merchantIds/{id} | 
[**merchant_ids_get_collection**](MerchantIdsApi.md#merchant_ids_get_collection) | **GET** /v1/merchantIds | 
[**merchant_ids_get_instance**](MerchantIdsApi.md#merchant_ids_get_instance) | **GET** /v1/merchantIds/{id} | 
[**merchant_ids_update_instance**](MerchantIdsApi.md#merchant_ids_update_instance) | **PATCH** /v1/merchantIds/{id} | 


# **merchant_ids_certificates_get_to_many_related**
> CertificatesResponse merchant_ids_certificates_get_to_many_related(id, filter_display_name=filter_display_name, filter_certificate_type=filter_certificate_type, filter_serial_number=filter_serial_number, filter_id=filter_id, sort=sort, fields_certificates=fields_certificates, fields_pass_type_ids=fields_pass_type_ids, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.certificates_response import CertificatesResponse
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
    api_instance = openapi_client.MerchantIdsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_display_name = ['filter_display_name_example'] # List[str] | filter by attribute 'displayName' (optional)
    filter_certificate_type = ['filter_certificate_type_example'] # List[str] | filter by attribute 'certificateType' (optional)
    filter_serial_number = ['filter_serial_number_example'] # List[str] | filter by attribute 'serialNumber' (optional)
    filter_id = ['filter_id_example'] # List[str] | filter by id(s) (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; resources will be sorted as specified (optional)
    fields_certificates = ['fields_certificates_example'] # List[str] | the fields to include for returned resources of type certificates (optional)
    fields_pass_type_ids = ['fields_pass_type_ids_example'] # List[str] | the fields to include for returned resources of type passTypeIds (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.merchant_ids_certificates_get_to_many_related(id, filter_display_name=filter_display_name, filter_certificate_type=filter_certificate_type, filter_serial_number=filter_serial_number, filter_id=filter_id, sort=sort, fields_certificates=fields_certificates, fields_pass_type_ids=fields_pass_type_ids, limit=limit, include=include)
        print("The response of MerchantIdsApi->merchant_ids_certificates_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MerchantIdsApi->merchant_ids_certificates_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_display_name** | [**List[str]**](str.md)| filter by attribute &#39;displayName&#39; | [optional] 
 **filter_certificate_type** | [**List[str]**](str.md)| filter by attribute &#39;certificateType&#39; | [optional] 
 **filter_serial_number** | [**List[str]**](str.md)| filter by attribute &#39;serialNumber&#39; | [optional] 
 **filter_id** | [**List[str]**](str.md)| filter by id(s) | [optional] 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; resources will be sorted as specified | [optional] 
 **fields_certificates** | [**List[str]**](str.md)| the fields to include for returned resources of type certificates | [optional] 
 **fields_pass_type_ids** | [**List[str]**](str.md)| the fields to include for returned resources of type passTypeIds | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**CertificatesResponse**](CertificatesResponse.md)

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
**200** | List of Certificates |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **merchant_ids_certificates_get_to_many_relationship**
> MerchantIdCertificatesLinkagesResponse merchant_ids_certificates_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.merchant_id_certificates_linkages_response import MerchantIdCertificatesLinkagesResponse
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
    api_instance = openapi_client.MerchantIdsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.merchant_ids_certificates_get_to_many_relationship(id, limit=limit)
        print("The response of MerchantIdsApi->merchant_ids_certificates_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MerchantIdsApi->merchant_ids_certificates_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**MerchantIdCertificatesLinkagesResponse**](MerchantIdCertificatesLinkagesResponse.md)

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

# **merchant_ids_create_instance**
> MerchantIdResponse merchant_ids_create_instance(merchant_id_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.merchant_id_create_request import MerchantIdCreateRequest
from openapi_client.models.merchant_id_response import MerchantIdResponse
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
    api_instance = openapi_client.MerchantIdsApi(api_client)
    merchant_id_create_request = openapi_client.MerchantIdCreateRequest() # MerchantIdCreateRequest | MerchantId representation

    try:
        api_response = api_instance.merchant_ids_create_instance(merchant_id_create_request)
        print("The response of MerchantIdsApi->merchant_ids_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MerchantIdsApi->merchant_ids_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **merchant_id_create_request** | [**MerchantIdCreateRequest**](MerchantIdCreateRequest.md)| MerchantId representation | 

### Return type

[**MerchantIdResponse**](MerchantIdResponse.md)

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
**201** | Single MerchantId |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **merchant_ids_delete_instance**
> merchant_ids_delete_instance(id)

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
    api_instance = openapi_client.MerchantIdsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.merchant_ids_delete_instance(id)
    except Exception as e:
        print("Exception when calling MerchantIdsApi->merchant_ids_delete_instance: %s\n" % e)
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

# **merchant_ids_get_collection**
> MerchantIdsResponse merchant_ids_get_collection(filter_name=filter_name, filter_identifier=filter_identifier, sort=sort, fields_merchant_ids=fields_merchant_ids, fields_certificates=fields_certificates, limit=limit, include=include, limit_certificates=limit_certificates)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.merchant_ids_response import MerchantIdsResponse
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
    api_instance = openapi_client.MerchantIdsApi(api_client)
    filter_name = ['filter_name_example'] # List[str] | filter by attribute 'name' (optional)
    filter_identifier = ['filter_identifier_example'] # List[str] | filter by attribute 'identifier' (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; resources will be sorted as specified (optional)
    fields_merchant_ids = ['fields_merchant_ids_example'] # List[str] | the fields to include for returned resources of type merchantIds (optional)
    fields_certificates = ['fields_certificates_example'] # List[str] | the fields to include for returned resources of type certificates (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_certificates = 56 # int | maximum number of related certificates returned (when they are included) (optional)

    try:
        api_response = api_instance.merchant_ids_get_collection(filter_name=filter_name, filter_identifier=filter_identifier, sort=sort, fields_merchant_ids=fields_merchant_ids, fields_certificates=fields_certificates, limit=limit, include=include, limit_certificates=limit_certificates)
        print("The response of MerchantIdsApi->merchant_ids_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MerchantIdsApi->merchant_ids_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter_name** | [**List[str]**](str.md)| filter by attribute &#39;name&#39; | [optional] 
 **filter_identifier** | [**List[str]**](str.md)| filter by attribute &#39;identifier&#39; | [optional] 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; resources will be sorted as specified | [optional] 
 **fields_merchant_ids** | [**List[str]**](str.md)| the fields to include for returned resources of type merchantIds | [optional] 
 **fields_certificates** | [**List[str]**](str.md)| the fields to include for returned resources of type certificates | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_certificates** | **int**| maximum number of related certificates returned (when they are included) | [optional] 

### Return type

[**MerchantIdsResponse**](MerchantIdsResponse.md)

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
**200** | List of MerchantIds |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **merchant_ids_get_instance**
> MerchantIdResponse merchant_ids_get_instance(id, fields_merchant_ids=fields_merchant_ids, fields_certificates=fields_certificates, include=include, limit_certificates=limit_certificates)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.merchant_id_response import MerchantIdResponse
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
    api_instance = openapi_client.MerchantIdsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_merchant_ids = ['fields_merchant_ids_example'] # List[str] | the fields to include for returned resources of type merchantIds (optional)
    fields_certificates = ['fields_certificates_example'] # List[str] | the fields to include for returned resources of type certificates (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_certificates = 56 # int | maximum number of related certificates returned (when they are included) (optional)

    try:
        api_response = api_instance.merchant_ids_get_instance(id, fields_merchant_ids=fields_merchant_ids, fields_certificates=fields_certificates, include=include, limit_certificates=limit_certificates)
        print("The response of MerchantIdsApi->merchant_ids_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MerchantIdsApi->merchant_ids_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_merchant_ids** | [**List[str]**](str.md)| the fields to include for returned resources of type merchantIds | [optional] 
 **fields_certificates** | [**List[str]**](str.md)| the fields to include for returned resources of type certificates | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_certificates** | **int**| maximum number of related certificates returned (when they are included) | [optional] 

### Return type

[**MerchantIdResponse**](MerchantIdResponse.md)

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
**200** | Single MerchantId |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **merchant_ids_update_instance**
> MerchantIdResponse merchant_ids_update_instance(id, merchant_id_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.merchant_id_response import MerchantIdResponse
from openapi_client.models.merchant_id_update_request import MerchantIdUpdateRequest
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
    api_instance = openapi_client.MerchantIdsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    merchant_id_update_request = openapi_client.MerchantIdUpdateRequest() # MerchantIdUpdateRequest | MerchantId representation

    try:
        api_response = api_instance.merchant_ids_update_instance(id, merchant_id_update_request)
        print("The response of MerchantIdsApi->merchant_ids_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MerchantIdsApi->merchant_ids_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **merchant_id_update_request** | [**MerchantIdUpdateRequest**](MerchantIdUpdateRequest.md)| MerchantId representation | 

### Return type

[**MerchantIdResponse**](MerchantIdResponse.md)

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
**200** | Single MerchantId |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

