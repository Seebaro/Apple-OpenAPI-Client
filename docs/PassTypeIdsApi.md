# openapi_client.PassTypeIdsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**pass_type_ids_certificates_get_to_many_related**](PassTypeIdsApi.md#pass_type_ids_certificates_get_to_many_related) | **GET** /v1/passTypeIds/{id}/certificates | 
[**pass_type_ids_certificates_get_to_many_relationship**](PassTypeIdsApi.md#pass_type_ids_certificates_get_to_many_relationship) | **GET** /v1/passTypeIds/{id}/relationships/certificates | 
[**pass_type_ids_create_instance**](PassTypeIdsApi.md#pass_type_ids_create_instance) | **POST** /v1/passTypeIds | 
[**pass_type_ids_delete_instance**](PassTypeIdsApi.md#pass_type_ids_delete_instance) | **DELETE** /v1/passTypeIds/{id} | 
[**pass_type_ids_get_collection**](PassTypeIdsApi.md#pass_type_ids_get_collection) | **GET** /v1/passTypeIds | 
[**pass_type_ids_get_instance**](PassTypeIdsApi.md#pass_type_ids_get_instance) | **GET** /v1/passTypeIds/{id} | 
[**pass_type_ids_update_instance**](PassTypeIdsApi.md#pass_type_ids_update_instance) | **PATCH** /v1/passTypeIds/{id} | 


# **pass_type_ids_certificates_get_to_many_related**
> CertificatesResponse pass_type_ids_certificates_get_to_many_related(id, filter_display_name=filter_display_name, filter_certificate_type=filter_certificate_type, filter_serial_number=filter_serial_number, filter_id=filter_id, sort=sort, fields_certificates=fields_certificates, fields_pass_type_ids=fields_pass_type_ids, limit=limit, include=include)

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
    api_instance = openapi_client.PassTypeIdsApi(api_client)
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
        api_response = api_instance.pass_type_ids_certificates_get_to_many_related(id, filter_display_name=filter_display_name, filter_certificate_type=filter_certificate_type, filter_serial_number=filter_serial_number, filter_id=filter_id, sort=sort, fields_certificates=fields_certificates, fields_pass_type_ids=fields_pass_type_ids, limit=limit, include=include)
        print("The response of PassTypeIdsApi->pass_type_ids_certificates_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PassTypeIdsApi->pass_type_ids_certificates_get_to_many_related: %s\n" % e)
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

# **pass_type_ids_certificates_get_to_many_relationship**
> PassTypeIdCertificatesLinkagesResponse pass_type_ids_certificates_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.pass_type_id_certificates_linkages_response import PassTypeIdCertificatesLinkagesResponse
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
    api_instance = openapi_client.PassTypeIdsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.pass_type_ids_certificates_get_to_many_relationship(id, limit=limit)
        print("The response of PassTypeIdsApi->pass_type_ids_certificates_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PassTypeIdsApi->pass_type_ids_certificates_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**PassTypeIdCertificatesLinkagesResponse**](PassTypeIdCertificatesLinkagesResponse.md)

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

# **pass_type_ids_create_instance**
> PassTypeIdResponse pass_type_ids_create_instance(pass_type_id_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.pass_type_id_create_request import PassTypeIdCreateRequest
from openapi_client.models.pass_type_id_response import PassTypeIdResponse
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
    api_instance = openapi_client.PassTypeIdsApi(api_client)
    pass_type_id_create_request = openapi_client.PassTypeIdCreateRequest() # PassTypeIdCreateRequest | PassTypeId representation

    try:
        api_response = api_instance.pass_type_ids_create_instance(pass_type_id_create_request)
        print("The response of PassTypeIdsApi->pass_type_ids_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PassTypeIdsApi->pass_type_ids_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pass_type_id_create_request** | [**PassTypeIdCreateRequest**](PassTypeIdCreateRequest.md)| PassTypeId representation | 

### Return type

[**PassTypeIdResponse**](PassTypeIdResponse.md)

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
**201** | Single PassTypeId |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **pass_type_ids_delete_instance**
> pass_type_ids_delete_instance(id)

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
    api_instance = openapi_client.PassTypeIdsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.pass_type_ids_delete_instance(id)
    except Exception as e:
        print("Exception when calling PassTypeIdsApi->pass_type_ids_delete_instance: %s\n" % e)
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

# **pass_type_ids_get_collection**
> PassTypeIdsResponse pass_type_ids_get_collection(filter_name=filter_name, filter_identifier=filter_identifier, filter_id=filter_id, sort=sort, fields_pass_type_ids=fields_pass_type_ids, fields_certificates=fields_certificates, limit=limit, include=include, limit_certificates=limit_certificates)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.pass_type_ids_response import PassTypeIdsResponse
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
    api_instance = openapi_client.PassTypeIdsApi(api_client)
    filter_name = ['filter_name_example'] # List[str] | filter by attribute 'name' (optional)
    filter_identifier = ['filter_identifier_example'] # List[str] | filter by attribute 'identifier' (optional)
    filter_id = ['filter_id_example'] # List[str] | filter by id(s) (optional)
    sort = ['sort_example'] # List[str] | comma-separated list of sort expressions; resources will be sorted as specified (optional)
    fields_pass_type_ids = ['fields_pass_type_ids_example'] # List[str] | the fields to include for returned resources of type passTypeIds (optional)
    fields_certificates = ['fields_certificates_example'] # List[str] | the fields to include for returned resources of type certificates (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_certificates = 56 # int | maximum number of related certificates returned (when they are included) (optional)

    try:
        api_response = api_instance.pass_type_ids_get_collection(filter_name=filter_name, filter_identifier=filter_identifier, filter_id=filter_id, sort=sort, fields_pass_type_ids=fields_pass_type_ids, fields_certificates=fields_certificates, limit=limit, include=include, limit_certificates=limit_certificates)
        print("The response of PassTypeIdsApi->pass_type_ids_get_collection:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PassTypeIdsApi->pass_type_ids_get_collection: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter_name** | [**List[str]**](str.md)| filter by attribute &#39;name&#39; | [optional] 
 **filter_identifier** | [**List[str]**](str.md)| filter by attribute &#39;identifier&#39; | [optional] 
 **filter_id** | [**List[str]**](str.md)| filter by id(s) | [optional] 
 **sort** | [**List[str]**](str.md)| comma-separated list of sort expressions; resources will be sorted as specified | [optional] 
 **fields_pass_type_ids** | [**List[str]**](str.md)| the fields to include for returned resources of type passTypeIds | [optional] 
 **fields_certificates** | [**List[str]**](str.md)| the fields to include for returned resources of type certificates | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_certificates** | **int**| maximum number of related certificates returned (when they are included) | [optional] 

### Return type

[**PassTypeIdsResponse**](PassTypeIdsResponse.md)

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
**200** | List of PassTypeIds |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **pass_type_ids_get_instance**
> PassTypeIdResponse pass_type_ids_get_instance(id, fields_pass_type_ids=fields_pass_type_ids, fields_certificates=fields_certificates, include=include, limit_certificates=limit_certificates)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.pass_type_id_response import PassTypeIdResponse
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
    api_instance = openapi_client.PassTypeIdsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_pass_type_ids = ['fields_pass_type_ids_example'] # List[str] | the fields to include for returned resources of type passTypeIds (optional)
    fields_certificates = ['fields_certificates_example'] # List[str] | the fields to include for returned resources of type certificates (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_certificates = 56 # int | maximum number of related certificates returned (when they are included) (optional)

    try:
        api_response = api_instance.pass_type_ids_get_instance(id, fields_pass_type_ids=fields_pass_type_ids, fields_certificates=fields_certificates, include=include, limit_certificates=limit_certificates)
        print("The response of PassTypeIdsApi->pass_type_ids_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PassTypeIdsApi->pass_type_ids_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_pass_type_ids** | [**List[str]**](str.md)| the fields to include for returned resources of type passTypeIds | [optional] 
 **fields_certificates** | [**List[str]**](str.md)| the fields to include for returned resources of type certificates | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_certificates** | **int**| maximum number of related certificates returned (when they are included) | [optional] 

### Return type

[**PassTypeIdResponse**](PassTypeIdResponse.md)

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
**200** | Single PassTypeId |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **pass_type_ids_update_instance**
> PassTypeIdResponse pass_type_ids_update_instance(id, pass_type_id_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.pass_type_id_response import PassTypeIdResponse
from openapi_client.models.pass_type_id_update_request import PassTypeIdUpdateRequest
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
    api_instance = openapi_client.PassTypeIdsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    pass_type_id_update_request = openapi_client.PassTypeIdUpdateRequest() # PassTypeIdUpdateRequest | PassTypeId representation

    try:
        api_response = api_instance.pass_type_ids_update_instance(id, pass_type_id_update_request)
        print("The response of PassTypeIdsApi->pass_type_ids_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PassTypeIdsApi->pass_type_ids_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **pass_type_id_update_request** | [**PassTypeIdUpdateRequest**](PassTypeIdUpdateRequest.md)| PassTypeId representation | 

### Return type

[**PassTypeIdResponse**](PassTypeIdResponse.md)

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
**200** | Single PassTypeId |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

