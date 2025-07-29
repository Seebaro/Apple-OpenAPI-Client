# openapi_client.GameCenterActivityLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_activity_localizations_create_instance**](GameCenterActivityLocalizationsApi.md#game_center_activity_localizations_create_instance) | **POST** /v1/gameCenterActivityLocalizations | 
[**game_center_activity_localizations_delete_instance**](GameCenterActivityLocalizationsApi.md#game_center_activity_localizations_delete_instance) | **DELETE** /v1/gameCenterActivityLocalizations/{id} | 
[**game_center_activity_localizations_get_instance**](GameCenterActivityLocalizationsApi.md#game_center_activity_localizations_get_instance) | **GET** /v1/gameCenterActivityLocalizations/{id} | 
[**game_center_activity_localizations_image_get_to_one_related**](GameCenterActivityLocalizationsApi.md#game_center_activity_localizations_image_get_to_one_related) | **GET** /v1/gameCenterActivityLocalizations/{id}/image | 
[**game_center_activity_localizations_image_get_to_one_relationship**](GameCenterActivityLocalizationsApi.md#game_center_activity_localizations_image_get_to_one_relationship) | **GET** /v1/gameCenterActivityLocalizations/{id}/relationships/image | 
[**game_center_activity_localizations_update_instance**](GameCenterActivityLocalizationsApi.md#game_center_activity_localizations_update_instance) | **PATCH** /v1/gameCenterActivityLocalizations/{id} | 


# **game_center_activity_localizations_create_instance**
> GameCenterActivityLocalizationResponse game_center_activity_localizations_create_instance(game_center_activity_localization_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_activity_localization_create_request import GameCenterActivityLocalizationCreateRequest
from openapi_client.models.game_center_activity_localization_response import GameCenterActivityLocalizationResponse
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
    api_instance = openapi_client.GameCenterActivityLocalizationsApi(api_client)
    game_center_activity_localization_create_request = openapi_client.GameCenterActivityLocalizationCreateRequest() # GameCenterActivityLocalizationCreateRequest | GameCenterActivityLocalization representation

    try:
        api_response = api_instance.game_center_activity_localizations_create_instance(game_center_activity_localization_create_request)
        print("The response of GameCenterActivityLocalizationsApi->game_center_activity_localizations_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterActivityLocalizationsApi->game_center_activity_localizations_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_activity_localization_create_request** | [**GameCenterActivityLocalizationCreateRequest**](GameCenterActivityLocalizationCreateRequest.md)| GameCenterActivityLocalization representation | 

### Return type

[**GameCenterActivityLocalizationResponse**](GameCenterActivityLocalizationResponse.md)

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
**201** | Single GameCenterActivityLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_activity_localizations_delete_instance**
> game_center_activity_localizations_delete_instance(id)

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
    api_instance = openapi_client.GameCenterActivityLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.game_center_activity_localizations_delete_instance(id)
    except Exception as e:
        print("Exception when calling GameCenterActivityLocalizationsApi->game_center_activity_localizations_delete_instance: %s\n" % e)
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

# **game_center_activity_localizations_get_instance**
> GameCenterActivityLocalizationResponse game_center_activity_localizations_get_instance(id, fields_game_center_activity_localizations=fields_game_center_activity_localizations, fields_game_center_activity_images=fields_game_center_activity_images, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_activity_localization_response import GameCenterActivityLocalizationResponse
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
    api_instance = openapi_client.GameCenterActivityLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_activity_localizations = ['fields_game_center_activity_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterActivityLocalizations (optional)
    fields_game_center_activity_images = ['fields_game_center_activity_images_example'] # List[str] | the fields to include for returned resources of type gameCenterActivityImages (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_activity_localizations_get_instance(id, fields_game_center_activity_localizations=fields_game_center_activity_localizations, fields_game_center_activity_images=fields_game_center_activity_images, include=include)
        print("The response of GameCenterActivityLocalizationsApi->game_center_activity_localizations_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterActivityLocalizationsApi->game_center_activity_localizations_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_activity_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivityLocalizations | [optional] 
 **fields_game_center_activity_images** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivityImages | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**GameCenterActivityLocalizationResponse**](GameCenterActivityLocalizationResponse.md)

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
**200** | Single GameCenterActivityLocalization |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_activity_localizations_image_get_to_one_related**
> GameCenterActivityImageResponse game_center_activity_localizations_image_get_to_one_related(id, fields_game_center_activity_images=fields_game_center_activity_images)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_activity_image_response import GameCenterActivityImageResponse
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
    api_instance = openapi_client.GameCenterActivityLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_activity_images = ['fields_game_center_activity_images_example'] # List[str] | the fields to include for returned resources of type gameCenterActivityImages (optional)

    try:
        api_response = api_instance.game_center_activity_localizations_image_get_to_one_related(id, fields_game_center_activity_images=fields_game_center_activity_images)
        print("The response of GameCenterActivityLocalizationsApi->game_center_activity_localizations_image_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterActivityLocalizationsApi->game_center_activity_localizations_image_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_activity_images** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivityImages | [optional] 

### Return type

[**GameCenterActivityImageResponse**](GameCenterActivityImageResponse.md)

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
**200** | Single GameCenterActivityImage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_activity_localizations_image_get_to_one_relationship**
> GameCenterActivityLocalizationImageLinkageResponse game_center_activity_localizations_image_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_activity_localization_image_linkage_response import GameCenterActivityLocalizationImageLinkageResponse
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
    api_instance = openapi_client.GameCenterActivityLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.game_center_activity_localizations_image_get_to_one_relationship(id)
        print("The response of GameCenterActivityLocalizationsApi->game_center_activity_localizations_image_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterActivityLocalizationsApi->game_center_activity_localizations_image_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**GameCenterActivityLocalizationImageLinkageResponse**](GameCenterActivityLocalizationImageLinkageResponse.md)

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

# **game_center_activity_localizations_update_instance**
> GameCenterActivityLocalizationResponse game_center_activity_localizations_update_instance(id, game_center_activity_localization_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_activity_localization_response import GameCenterActivityLocalizationResponse
from openapi_client.models.game_center_activity_localization_update_request import GameCenterActivityLocalizationUpdateRequest
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
    api_instance = openapi_client.GameCenterActivityLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_activity_localization_update_request = openapi_client.GameCenterActivityLocalizationUpdateRequest() # GameCenterActivityLocalizationUpdateRequest | GameCenterActivityLocalization representation

    try:
        api_response = api_instance.game_center_activity_localizations_update_instance(id, game_center_activity_localization_update_request)
        print("The response of GameCenterActivityLocalizationsApi->game_center_activity_localizations_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterActivityLocalizationsApi->game_center_activity_localizations_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_activity_localization_update_request** | [**GameCenterActivityLocalizationUpdateRequest**](GameCenterActivityLocalizationUpdateRequest.md)| GameCenterActivityLocalization representation | 

### Return type

[**GameCenterActivityLocalizationResponse**](GameCenterActivityLocalizationResponse.md)

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
**200** | Single GameCenterActivityLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

