# openapi_client.GameCenterLeaderboardSetImagesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_leaderboard_set_images_create_instance**](GameCenterLeaderboardSetImagesApi.md#game_center_leaderboard_set_images_create_instance) | **POST** /v1/gameCenterLeaderboardSetImages | 
[**game_center_leaderboard_set_images_delete_instance**](GameCenterLeaderboardSetImagesApi.md#game_center_leaderboard_set_images_delete_instance) | **DELETE** /v1/gameCenterLeaderboardSetImages/{id} | 
[**game_center_leaderboard_set_images_get_instance**](GameCenterLeaderboardSetImagesApi.md#game_center_leaderboard_set_images_get_instance) | **GET** /v1/gameCenterLeaderboardSetImages/{id} | 
[**game_center_leaderboard_set_images_update_instance**](GameCenterLeaderboardSetImagesApi.md#game_center_leaderboard_set_images_update_instance) | **PATCH** /v1/gameCenterLeaderboardSetImages/{id} | 


# **game_center_leaderboard_set_images_create_instance**
> GameCenterLeaderboardSetImageResponse game_center_leaderboard_set_images_create_instance(game_center_leaderboard_set_image_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_image_create_request import GameCenterLeaderboardSetImageCreateRequest
from openapi_client.models.game_center_leaderboard_set_image_response import GameCenterLeaderboardSetImageResponse
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
    api_instance = openapi_client.GameCenterLeaderboardSetImagesApi(api_client)
    game_center_leaderboard_set_image_create_request = openapi_client.GameCenterLeaderboardSetImageCreateRequest() # GameCenterLeaderboardSetImageCreateRequest | GameCenterLeaderboardSetImage representation

    try:
        api_response = api_instance.game_center_leaderboard_set_images_create_instance(game_center_leaderboard_set_image_create_request)
        print("The response of GameCenterLeaderboardSetImagesApi->game_center_leaderboard_set_images_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetImagesApi->game_center_leaderboard_set_images_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_leaderboard_set_image_create_request** | [**GameCenterLeaderboardSetImageCreateRequest**](GameCenterLeaderboardSetImageCreateRequest.md)| GameCenterLeaderboardSetImage representation | 

### Return type

[**GameCenterLeaderboardSetImageResponse**](GameCenterLeaderboardSetImageResponse.md)

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
**201** | Single GameCenterLeaderboardSetImage |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_leaderboard_set_images_delete_instance**
> game_center_leaderboard_set_images_delete_instance(id)

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
    api_instance = openapi_client.GameCenterLeaderboardSetImagesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.game_center_leaderboard_set_images_delete_instance(id)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetImagesApi->game_center_leaderboard_set_images_delete_instance: %s\n" % e)
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

# **game_center_leaderboard_set_images_get_instance**
> GameCenterLeaderboardSetImageResponse game_center_leaderboard_set_images_get_instance(id, fields_game_center_leaderboard_set_images=fields_game_center_leaderboard_set_images, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_image_response import GameCenterLeaderboardSetImageResponse
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
    api_instance = openapi_client.GameCenterLeaderboardSetImagesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_leaderboard_set_images = ['fields_game_center_leaderboard_set_images_example'] # List[str] | the fields to include for returned resources of type gameCenterLeaderboardSetImages (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_leaderboard_set_images_get_instance(id, fields_game_center_leaderboard_set_images=fields_game_center_leaderboard_set_images, include=include)
        print("The response of GameCenterLeaderboardSetImagesApi->game_center_leaderboard_set_images_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetImagesApi->game_center_leaderboard_set_images_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_leaderboard_set_images** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterLeaderboardSetImages | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**GameCenterLeaderboardSetImageResponse**](GameCenterLeaderboardSetImageResponse.md)

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
**200** | Single GameCenterLeaderboardSetImage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_leaderboard_set_images_update_instance**
> GameCenterLeaderboardSetImageResponse game_center_leaderboard_set_images_update_instance(id, game_center_leaderboard_set_image_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_leaderboard_set_image_response import GameCenterLeaderboardSetImageResponse
from openapi_client.models.game_center_leaderboard_set_image_update_request import GameCenterLeaderboardSetImageUpdateRequest
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
    api_instance = openapi_client.GameCenterLeaderboardSetImagesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_leaderboard_set_image_update_request = openapi_client.GameCenterLeaderboardSetImageUpdateRequest() # GameCenterLeaderboardSetImageUpdateRequest | GameCenterLeaderboardSetImage representation

    try:
        api_response = api_instance.game_center_leaderboard_set_images_update_instance(id, game_center_leaderboard_set_image_update_request)
        print("The response of GameCenterLeaderboardSetImagesApi->game_center_leaderboard_set_images_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterLeaderboardSetImagesApi->game_center_leaderboard_set_images_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_leaderboard_set_image_update_request** | [**GameCenterLeaderboardSetImageUpdateRequest**](GameCenterLeaderboardSetImageUpdateRequest.md)| GameCenterLeaderboardSetImage representation | 

### Return type

[**GameCenterLeaderboardSetImageResponse**](GameCenterLeaderboardSetImageResponse.md)

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
**200** | Single GameCenterLeaderboardSetImage |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

