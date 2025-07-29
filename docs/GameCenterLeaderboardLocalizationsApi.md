# openapi_client.GameCenterLeaderboardLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_leaderboard_localizations_create_instance**](GameCenterLeaderboardLocalizationsApi.md#game_center_leaderboard_localizations_create_instance) | **POST** /v1/gameCenterLeaderboardLocalizations | 
[**game_center_leaderboard_localizations_delete_instance**](GameCenterLeaderboardLocalizationsApi.md#game_center_leaderboard_localizations_delete_instance) | **DELETE** /v1/gameCenterLeaderboardLocalizations/{id} | 
[**game_center_leaderboard_localizations_game_center_leaderboard_image_get_to_one_related**](GameCenterLeaderboardLocalizationsApi.md#game_center_leaderboard_localizations_game_center_leaderboard_image_get_to_one_related) | **GET** /v1/gameCenterLeaderboardLocalizations/{id}/gameCenterLeaderboardImage | 
[**game_center_leaderboard_localizations_game_center_leaderboard_image_get_to_one_relationship**](GameCenterLeaderboardLocalizationsApi.md#game_center_leaderboard_localizations_game_center_leaderboard_image_get_to_one_relationship) | **GET** /v1/gameCenterLeaderboardLocalizations/{id}/relationships/gameCenterLeaderboardImage | 
[**game_center_leaderboard_localizations_get_instance**](GameCenterLeaderboardLocalizationsApi.md#game_center_leaderboard_localizations_get_instance) | **GET** /v1/gameCenterLeaderboardLocalizations/{id} | 
[**game_center_leaderboard_localizations_update_instance**](GameCenterLeaderboardLocalizationsApi.md#game_center_leaderboard_localizations_update_instance) | **PATCH** /v1/gameCenterLeaderboardLocalizations/{id} | 


# **game_center_leaderboard_localizations_create_instance**
> GameCenterLeaderboardLocalizationResponse game_center_leaderboard_localizations_create_instance(game_center_leaderboard_localization_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_localization_create_request import GameCenterLeaderboardLocalizationCreateRequest
from openapi_client.models.game_center_leaderboard_localization_response import GameCenterLeaderboardLocalizationResponse
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
    api_instance = openapi_client.GameCenterLeaderboardLocalizationsApi(api_client)
    game_center_leaderboard_localization_create_request = openapi_client.GameCenterLeaderboardLocalizationCreateRequest() # GameCenterLeaderboardLocalizationCreateRequest | GameCenterLeaderboardLocalization representation

    try:
        api_response = api_instance.game_center_leaderboard_localizations_create_instance(game_center_leaderboard_localization_create_request)
        print("The response of GameCenterLeaderboardLocalizationsApi->game_center_leaderboard_localizations_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardLocalizationsApi->game_center_leaderboard_localizations_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_leaderboard_localization_create_request** | [**GameCenterLeaderboardLocalizationCreateRequest**](GameCenterLeaderboardLocalizationCreateRequest.md)| GameCenterLeaderboardLocalization representation | 

### Return type

[**GameCenterLeaderboardLocalizationResponse**](GameCenterLeaderboardLocalizationResponse.md)

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
**201** | Single GameCenterLeaderboardLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_leaderboard_localizations_delete_instance**
> game_center_leaderboard_localizations_delete_instance(id)

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
    api_instance = openapi_client.GameCenterLeaderboardLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.game_center_leaderboard_localizations_delete_instance(id)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardLocalizationsApi->game_center_leaderboard_localizations_delete_instance: %s\n" % e)
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

# **game_center_leaderboard_localizations_game_center_leaderboard_image_get_to_one_related**
> GameCenterLeaderboardImageResponse game_center_leaderboard_localizations_game_center_leaderboard_image_get_to_one_related(id, fields_game_center_leaderboard_images=fields_game_center_leaderboard_images, fields_game_center_leaderboard_localizations=fields_game_center_leaderboard_localizations, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_image_response import GameCenterLeaderboardImageResponse
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
    api_instance = openapi_client.GameCenterLeaderboardLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_leaderboard_images = ['fields_game_center_leaderboard_images_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardImages (optional)
    fields_game_center_leaderboard_localizations = ['fields_game_center_leaderboard_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardLocalizations (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_leaderboard_localizations_game_center_leaderboard_image_get_to_one_related(id, fields_game_center_leaderboard_images=fields_game_center_leaderboard_images, fields_game_center_leaderboard_localizations=fields_game_center_leaderboard_localizations, include=include)
        print("The response of GameCenterLeaderboardLocalizationsApi->game_center_leaderboard_localizations_game_center_leaderboard_image_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardLocalizationsApi->game_center_leaderboard_localizations_game_center_leaderboard_image_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_leaderboard_images** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardImages | [optional] 
 **fields_game_center_leaderboard_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**GameCenterLeaderboardImageResponse**](GameCenterLeaderboardImageResponse.md)

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
**200** | Single GameCenterLeaderboardImage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_leaderboard_localizations_game_center_leaderboard_image_get_to_one_relationship**
> GameCenterLeaderboardLocalizationGameCenterLeaderboardImageLinkageResponse game_center_leaderboard_localizations_game_center_leaderboard_image_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_localization_game_center_leaderboard_image_linkage_response import GameCenterLeaderboardLocalizationGameCenterLeaderboardImageLinkageResponse
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
    api_instance = openapi_client.GameCenterLeaderboardLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.game_center_leaderboard_localizations_game_center_leaderboard_image_get_to_one_relationship(id)
        print("The response of GameCenterLeaderboardLocalizationsApi->game_center_leaderboard_localizations_game_center_leaderboard_image_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardLocalizationsApi->game_center_leaderboard_localizations_game_center_leaderboard_image_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**GameCenterLeaderboardLocalizationGameCenterLeaderboardImageLinkageResponse**](GameCenterLeaderboardLocalizationGameCenterLeaderboardImageLinkageResponse.md)

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

# **game_center_leaderboard_localizations_get_instance**
> GameCenterLeaderboardLocalizationResponse game_center_leaderboard_localizations_get_instance(id, fields_game_center_leaderboard_localizations=fields_game_center_leaderboard_localizations, fields_game_center_leaderboard_images=fields_game_center_leaderboard_images, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_localization_response import GameCenterLeaderboardLocalizationResponse
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
    api_instance = openapi_client.GameCenterLeaderboardLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_leaderboard_localizations = ['fields_game_center_leaderboard_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardLocalizations (optional)
    fields_game_center_leaderboard_images = ['fields_game_center_leaderboard_images_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardImages (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_leaderboard_localizations_get_instance(id, fields_game_center_leaderboard_localizations=fields_game_center_leaderboard_localizations, fields_game_center_leaderboard_images=fields_game_center_leaderboard_images, include=include)
        print("The response of GameCenterLeaderboardLocalizationsApi->game_center_leaderboard_localizations_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardLocalizationsApi->game_center_leaderboard_localizations_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_leaderboard_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardLocalizations | [optional] 
 **fields_game_center_leaderboard_images** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardImages | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**GameCenterLeaderboardLocalizationResponse**](GameCenterLeaderboardLocalizationResponse.md)

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
**200** | Single GameCenterLeaderboardLocalization |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_leaderboard_localizations_update_instance**
> GameCenterLeaderboardLocalizationResponse game_center_leaderboard_localizations_update_instance(id, game_center_leaderboard_localization_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_localization_response import GameCenterLeaderboardLocalizationResponse
from openapi_client.models.game_center_leaderboard_localization_update_request import GameCenterLeaderboardLocalizationUpdateRequest
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
    api_instance = openapi_client.GameCenterLeaderboardLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_leaderboard_localization_update_request = openapi_client.GameCenterLeaderboardLocalizationUpdateRequest() # GameCenterLeaderboardLocalizationUpdateRequest | GameCenterLeaderboardLocalization representation

    try:
        api_response = api_instance.game_center_leaderboard_localizations_update_instance(id, game_center_leaderboard_localization_update_request)
        print("The response of GameCenterLeaderboardLocalizationsApi->game_center_leaderboard_localizations_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardLocalizationsApi->game_center_leaderboard_localizations_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_leaderboard_localization_update_request** | [**GameCenterLeaderboardLocalizationUpdateRequest**](GameCenterLeaderboardLocalizationUpdateRequest.md)| GameCenterLeaderboardLocalization representation | 

### Return type

[**GameCenterLeaderboardLocalizationResponse**](GameCenterLeaderboardLocalizationResponse.md)

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
**200** | Single GameCenterLeaderboardLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

