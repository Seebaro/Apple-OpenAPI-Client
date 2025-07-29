# openapi_client.GameCenterChallengeVersionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_challenge_versions_create_instance**](GameCenterChallengeVersionsApi.md#game_center_challenge_versions_create_instance) | **POST** /v1/gameCenterChallengeVersions | 
[**game_center_challenge_versions_default_image_get_to_one_related**](GameCenterChallengeVersionsApi.md#game_center_challenge_versions_default_image_get_to_one_related) | **GET** /v1/gameCenterChallengeVersions/{id}/defaultImage | 
[**game_center_challenge_versions_default_image_get_to_one_relationship**](GameCenterChallengeVersionsApi.md#game_center_challenge_versions_default_image_get_to_one_relationship) | **GET** /v1/gameCenterChallengeVersions/{id}/relationships/defaultImage | 
[**game_center_challenge_versions_get_instance**](GameCenterChallengeVersionsApi.md#game_center_challenge_versions_get_instance) | **GET** /v1/gameCenterChallengeVersions/{id} | 
[**game_center_challenge_versions_localizations_get_to_many_related**](GameCenterChallengeVersionsApi.md#game_center_challenge_versions_localizations_get_to_many_related) | **GET** /v1/gameCenterChallengeVersions/{id}/localizations | 
[**game_center_challenge_versions_localizations_get_to_many_relationship**](GameCenterChallengeVersionsApi.md#game_center_challenge_versions_localizations_get_to_many_relationship) | **GET** /v1/gameCenterChallengeVersions/{id}/relationships/localizations | 


# **game_center_challenge_versions_create_instance**
> GameCenterChallengeVersionResponse game_center_challenge_versions_create_instance(game_center_challenge_version_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_challenge_version_create_request import GameCenterChallengeVersionCreateRequest
from openapi_client.models.game_center_challenge_version_response import GameCenterChallengeVersionResponse
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
    api_instance = openapi_client.GameCenterChallengeVersionsApi(api_client)
    game_center_challenge_version_create_request = openapi_client.GameCenterChallengeVersionCreateRequest() # GameCenterChallengeVersionCreateRequest | GameCenterChallengeVersion representation

    try:
        api_response = api_instance.game_center_challenge_versions_create_instance(game_center_challenge_version_create_request)
        print("The response of GameCenterChallengeVersionsApi->game_center_challenge_versions_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterChallengeVersionsApi->game_center_challenge_versions_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_challenge_version_create_request** | [**GameCenterChallengeVersionCreateRequest**](GameCenterChallengeVersionCreateRequest.md)| GameCenterChallengeVersion representation | 

### Return type

[**GameCenterChallengeVersionResponse**](GameCenterChallengeVersionResponse.md)

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
**201** | Single GameCenterChallengeVersion |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_challenge_versions_default_image_get_to_one_related**
> GameCenterChallengeImageResponse game_center_challenge_versions_default_image_get_to_one_related(id, fields_game_center_challenge_images=fields_game_center_challenge_images)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_challenge_image_response import GameCenterChallengeImageResponse
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
    api_instance = openapi_client.GameCenterChallengeVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_challenge_images = ['fields_game_center_challenge_images_example'] # List[str] | the fields to include for returned resources of type gameCenterChallengeImages (optional)

    try:
        api_response = api_instance.game_center_challenge_versions_default_image_get_to_one_related(id, fields_game_center_challenge_images=fields_game_center_challenge_images)
        print("The response of GameCenterChallengeVersionsApi->game_center_challenge_versions_default_image_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterChallengeVersionsApi->game_center_challenge_versions_default_image_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_challenge_images** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallengeImages | [optional] 

### Return type

[**GameCenterChallengeImageResponse**](GameCenterChallengeImageResponse.md)

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
**200** | Single GameCenterChallengeImage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_challenge_versions_default_image_get_to_one_relationship**
> GameCenterChallengeVersionDefaultImageLinkageResponse game_center_challenge_versions_default_image_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_challenge_version_default_image_linkage_response import GameCenterChallengeVersionDefaultImageLinkageResponse
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
    api_instance = openapi_client.GameCenterChallengeVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.game_center_challenge_versions_default_image_get_to_one_relationship(id)
        print("The response of GameCenterChallengeVersionsApi->game_center_challenge_versions_default_image_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterChallengeVersionsApi->game_center_challenge_versions_default_image_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**GameCenterChallengeVersionDefaultImageLinkageResponse**](GameCenterChallengeVersionDefaultImageLinkageResponse.md)

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

# **game_center_challenge_versions_get_instance**
> GameCenterChallengeVersionResponse game_center_challenge_versions_get_instance(id, fields_game_center_challenge_versions=fields_game_center_challenge_versions, fields_game_center_challenge_localizations=fields_game_center_challenge_localizations, fields_game_center_challenge_images=fields_game_center_challenge_images, include=include, limit_localizations=limit_localizations, limit_releases=limit_releases)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_challenge_version_response import GameCenterChallengeVersionResponse
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
    api_instance = openapi_client.GameCenterChallengeVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_challenge_versions = ['fields_game_center_challenge_versions_example'] # List[str] | the fields to include for returned resources of type gameCenterChallengeVersions (optional)
    fields_game_center_challenge_localizations = ['fields_game_center_challenge_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterChallengeLocalizations (optional)
    fields_game_center_challenge_images = ['fields_game_center_challenge_images_example'] # List[str] | the fields to include for returned resources of type gameCenterChallengeImages (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_localizations = 56 # int | maximum number of related localizations returned (when they are included) (optional)
    limit_releases = 56 # int | maximum number of related releases returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_challenge_versions_get_instance(id, fields_game_center_challenge_versions=fields_game_center_challenge_versions, fields_game_center_challenge_localizations=fields_game_center_challenge_localizations, fields_game_center_challenge_images=fields_game_center_challenge_images, include=include, limit_localizations=limit_localizations, limit_releases=limit_releases)
        print("The response of GameCenterChallengeVersionsApi->game_center_challenge_versions_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterChallengeVersionsApi->game_center_challenge_versions_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_challenge_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallengeVersions | [optional] 
 **fields_game_center_challenge_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallengeLocalizations | [optional] 
 **fields_game_center_challenge_images** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallengeImages | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_localizations** | **int**| maximum number of related localizations returned (when they are included) | [optional] 
 **limit_releases** | **int**| maximum number of related releases returned (when they are included) | [optional] 

### Return type

[**GameCenterChallengeVersionResponse**](GameCenterChallengeVersionResponse.md)

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
**200** | Single GameCenterChallengeVersion |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_challenge_versions_localizations_get_to_many_related**
> GameCenterChallengeLocalizationsResponse game_center_challenge_versions_localizations_get_to_many_related(id, fields_game_center_challenge_localizations=fields_game_center_challenge_localizations, fields_game_center_challenge_versions=fields_game_center_challenge_versions, fields_game_center_challenge_images=fields_game_center_challenge_images, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_challenge_localizations_response import GameCenterChallengeLocalizationsResponse
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
    api_instance = openapi_client.GameCenterChallengeVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_challenge_localizations = ['fields_game_center_challenge_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterChallengeLocalizations (optional)
    fields_game_center_challenge_versions = ['fields_game_center_challenge_versions_example'] # List[str] | the fields to include for returned resources of type gameCenterChallengeVersions (optional)
    fields_game_center_challenge_images = ['fields_game_center_challenge_images_example'] # List[str] | the fields to include for returned resources of type gameCenterChallengeImages (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_challenge_versions_localizations_get_to_many_related(id, fields_game_center_challenge_localizations=fields_game_center_challenge_localizations, fields_game_center_challenge_versions=fields_game_center_challenge_versions, fields_game_center_challenge_images=fields_game_center_challenge_images, limit=limit, include=include)
        print("The response of GameCenterChallengeVersionsApi->game_center_challenge_versions_localizations_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterChallengeVersionsApi->game_center_challenge_versions_localizations_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_challenge_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallengeLocalizations | [optional] 
 **fields_game_center_challenge_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallengeVersions | [optional] 
 **fields_game_center_challenge_images** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallengeImages | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**GameCenterChallengeLocalizationsResponse**](GameCenterChallengeLocalizationsResponse.md)

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
**200** | List of GameCenterChallengeLocalizations |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_challenge_versions_localizations_get_to_many_relationship**
> GameCenterChallengeVersionLocalizationsLinkagesResponse game_center_challenge_versions_localizations_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_challenge_version_localizations_linkages_response import GameCenterChallengeVersionLocalizationsLinkagesResponse
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
    api_instance = openapi_client.GameCenterChallengeVersionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_challenge_versions_localizations_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterChallengeVersionsApi->game_center_challenge_versions_localizations_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterChallengeVersionsApi->game_center_challenge_versions_localizations_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterChallengeVersionLocalizationsLinkagesResponse**](GameCenterChallengeVersionLocalizationsLinkagesResponse.md)

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

