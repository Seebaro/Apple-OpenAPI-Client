# openapi_client.GameCenterAchievementLocalizationsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_achievement_localizations_create_instance**](GameCenterAchievementLocalizationsApi.md#game_center_achievement_localizations_create_instance) | **POST** /v1/gameCenterAchievementLocalizations | 
[**game_center_achievement_localizations_delete_instance**](GameCenterAchievementLocalizationsApi.md#game_center_achievement_localizations_delete_instance) | **DELETE** /v1/gameCenterAchievementLocalizations/{id} | 
[**game_center_achievement_localizations_game_center_achievement_get_to_one_related**](GameCenterAchievementLocalizationsApi.md#game_center_achievement_localizations_game_center_achievement_get_to_one_related) | **GET** /v1/gameCenterAchievementLocalizations/{id}/gameCenterAchievement | 
[**game_center_achievement_localizations_game_center_achievement_get_to_one_relationship**](GameCenterAchievementLocalizationsApi.md#game_center_achievement_localizations_game_center_achievement_get_to_one_relationship) | **GET** /v1/gameCenterAchievementLocalizations/{id}/relationships/gameCenterAchievement | 
[**game_center_achievement_localizations_game_center_achievement_image_get_to_one_related**](GameCenterAchievementLocalizationsApi.md#game_center_achievement_localizations_game_center_achievement_image_get_to_one_related) | **GET** /v1/gameCenterAchievementLocalizations/{id}/gameCenterAchievementImage | 
[**game_center_achievement_localizations_game_center_achievement_image_get_to_one_relationship**](GameCenterAchievementLocalizationsApi.md#game_center_achievement_localizations_game_center_achievement_image_get_to_one_relationship) | **GET** /v1/gameCenterAchievementLocalizations/{id}/relationships/gameCenterAchievementImage | 
[**game_center_achievement_localizations_get_instance**](GameCenterAchievementLocalizationsApi.md#game_center_achievement_localizations_get_instance) | **GET** /v1/gameCenterAchievementLocalizations/{id} | 
[**game_center_achievement_localizations_update_instance**](GameCenterAchievementLocalizationsApi.md#game_center_achievement_localizations_update_instance) | **PATCH** /v1/gameCenterAchievementLocalizations/{id} | 


# **game_center_achievement_localizations_create_instance**
> GameCenterAchievementLocalizationResponse game_center_achievement_localizations_create_instance(game_center_achievement_localization_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_localization_create_request import GameCenterAchievementLocalizationCreateRequest
from openapi_client.models.game_center_achievement_localization_response import GameCenterAchievementLocalizationResponse
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
    api_instance = openapi_client.GameCenterAchievementLocalizationsApi(api_client)
    game_center_achievement_localization_create_request = openapi_client.GameCenterAchievementLocalizationCreateRequest() # GameCenterAchievementLocalizationCreateRequest | GameCenterAchievementLocalization representation

    try:
        api_response = api_instance.game_center_achievement_localizations_create_instance(game_center_achievement_localization_create_request)
        print("The response of GameCenterAchievementLocalizationsApi->game_center_achievement_localizations_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAchievementLocalizationsApi->game_center_achievement_localizations_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_achievement_localization_create_request** | [**GameCenterAchievementLocalizationCreateRequest**](GameCenterAchievementLocalizationCreateRequest.md)| GameCenterAchievementLocalization representation | 

### Return type

[**GameCenterAchievementLocalizationResponse**](GameCenterAchievementLocalizationResponse.md)

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
**201** | Single GameCenterAchievementLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_achievement_localizations_delete_instance**
> game_center_achievement_localizations_delete_instance(id)

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
    api_instance = openapi_client.GameCenterAchievementLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.game_center_achievement_localizations_delete_instance(id)
    except Exception as e:
        print("Exception when calling GameCenterAchievementLocalizationsApi->game_center_achievement_localizations_delete_instance: %s\n" % e)
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

# **game_center_achievement_localizations_game_center_achievement_get_to_one_related**
> GameCenterAchievementResponse game_center_achievement_localizations_game_center_achievement_get_to_one_related(id, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_achievement_localizations=fields_game_center_achievement_localizations, fields_game_center_achievement_releases=fields_game_center_achievement_releases, fields_game_center_activities=fields_game_center_activities, include=include, limit_localizations=limit_localizations, limit_releases=limit_releases)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_response import GameCenterAchievementResponse
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
    api_instance = openapi_client.GameCenterAchievementLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_achievements = ['fields_game_center_achievements_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievements (optional)
    fields_game_center_details = ['fields_game_center_details_example'] # List[str] | the fields to include for returned resources of type gameCenterDetails (optional)
    fields_game_center_groups = ['fields_game_center_groups_example'] # List[str] | the fields to include for returned resources of type gameCenterGroups (optional)
    fields_game_center_achievement_localizations = ['fields_game_center_achievement_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievementLocalizations (optional)
    fields_game_center_achievement_releases = ['fields_game_center_achievement_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievementReleases (optional)
    fields_game_center_activities = ['fields_game_center_activities_example'] # List[str] | the fields to include for returned resources of type gameCenterActivities (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_localizations = 56 # int | maximum number of related localizations returned (when they are included) (optional)
    limit_releases = 56 # int | maximum number of related releases returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_achievement_localizations_game_center_achievement_get_to_one_related(id, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_details=fields_game_center_details, fields_game_center_groups=fields_game_center_groups, fields_game_center_achievement_localizations=fields_game_center_achievement_localizations, fields_game_center_achievement_releases=fields_game_center_achievement_releases, fields_game_center_activities=fields_game_center_activities, include=include, limit_localizations=limit_localizations, limit_releases=limit_releases)
        print("The response of GameCenterAchievementLocalizationsApi->game_center_achievement_localizations_game_center_achievement_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAchievementLocalizationsApi->game_center_achievement_localizations_game_center_achievement_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_achievements** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievements | [optional] 
 **fields_game_center_details** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterDetails | [optional] 
 **fields_game_center_groups** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterGroups | [optional] 
 **fields_game_center_achievement_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional] 
 **fields_game_center_achievement_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievementReleases | [optional] 
 **fields_game_center_activities** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterActivities | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_localizations** | **int**| maximum number of related localizations returned (when they are included) | [optional] 
 **limit_releases** | **int**| maximum number of related releases returned (when they are included) | [optional] 

### Return type

[**GameCenterAchievementResponse**](GameCenterAchievementResponse.md)

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
**200** | Single GameCenterAchievement |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_achievement_localizations_game_center_achievement_get_to_one_relationship**
> GameCenterAchievementLocalizationGameCenterAchievementLinkageResponse game_center_achievement_localizations_game_center_achievement_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_localization_game_center_achievement_linkage_response import GameCenterAchievementLocalizationGameCenterAchievementLinkageResponse
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
    api_instance = openapi_client.GameCenterAchievementLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.game_center_achievement_localizations_game_center_achievement_get_to_one_relationship(id)
        print("The response of GameCenterAchievementLocalizationsApi->game_center_achievement_localizations_game_center_achievement_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAchievementLocalizationsApi->game_center_achievement_localizations_game_center_achievement_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**GameCenterAchievementLocalizationGameCenterAchievementLinkageResponse**](GameCenterAchievementLocalizationGameCenterAchievementLinkageResponse.md)

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

# **game_center_achievement_localizations_game_center_achievement_image_get_to_one_related**
> GameCenterAchievementImageResponse game_center_achievement_localizations_game_center_achievement_image_get_to_one_related(id, fields_game_center_achievement_images=fields_game_center_achievement_images, fields_game_center_achievement_localizations=fields_game_center_achievement_localizations, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_image_response import GameCenterAchievementImageResponse
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
    api_instance = openapi_client.GameCenterAchievementLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_achievement_images = ['fields_game_center_achievement_images_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievementImages (optional)
    fields_game_center_achievement_localizations = ['fields_game_center_achievement_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievementLocalizations (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_achievement_localizations_game_center_achievement_image_get_to_one_related(id, fields_game_center_achievement_images=fields_game_center_achievement_images, fields_game_center_achievement_localizations=fields_game_center_achievement_localizations, include=include)
        print("The response of GameCenterAchievementLocalizationsApi->game_center_achievement_localizations_game_center_achievement_image_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAchievementLocalizationsApi->game_center_achievement_localizations_game_center_achievement_image_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_achievement_images** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievementImages | [optional] 
 **fields_game_center_achievement_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**GameCenterAchievementImageResponse**](GameCenterAchievementImageResponse.md)

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
**200** | Single GameCenterAchievementImage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_achievement_localizations_game_center_achievement_image_get_to_one_relationship**
> GameCenterAchievementLocalizationGameCenterAchievementImageLinkageResponse game_center_achievement_localizations_game_center_achievement_image_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_localization_game_center_achievement_image_linkage_response import GameCenterAchievementLocalizationGameCenterAchievementImageLinkageResponse
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
    api_instance = openapi_client.GameCenterAchievementLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.game_center_achievement_localizations_game_center_achievement_image_get_to_one_relationship(id)
        print("The response of GameCenterAchievementLocalizationsApi->game_center_achievement_localizations_game_center_achievement_image_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAchievementLocalizationsApi->game_center_achievement_localizations_game_center_achievement_image_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**GameCenterAchievementLocalizationGameCenterAchievementImageLinkageResponse**](GameCenterAchievementLocalizationGameCenterAchievementImageLinkageResponse.md)

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

# **game_center_achievement_localizations_get_instance**
> GameCenterAchievementLocalizationResponse game_center_achievement_localizations_get_instance(id, fields_game_center_achievement_localizations=fields_game_center_achievement_localizations, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_achievement_images=fields_game_center_achievement_images, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_localization_response import GameCenterAchievementLocalizationResponse
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
    api_instance = openapi_client.GameCenterAchievementLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_achievement_localizations = ['fields_game_center_achievement_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievementLocalizations (optional)
    fields_game_center_achievements = ['fields_game_center_achievements_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievements (optional)
    fields_game_center_achievement_images = ['fields_game_center_achievement_images_example'] # List[str] | the fields to include for returned resources of type gameCenterAchievementImages (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_achievement_localizations_get_instance(id, fields_game_center_achievement_localizations=fields_game_center_achievement_localizations, fields_game_center_achievements=fields_game_center_achievements, fields_game_center_achievement_images=fields_game_center_achievement_images, include=include)
        print("The response of GameCenterAchievementLocalizationsApi->game_center_achievement_localizations_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAchievementLocalizationsApi->game_center_achievement_localizations_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_achievement_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievementLocalizations | [optional] 
 **fields_game_center_achievements** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievements | [optional] 
 **fields_game_center_achievement_images** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterAchievementImages | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**GameCenterAchievementLocalizationResponse**](GameCenterAchievementLocalizationResponse.md)

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
**200** | Single GameCenterAchievementLocalization |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_achievement_localizations_update_instance**
> GameCenterAchievementLocalizationResponse game_center_achievement_localizations_update_instance(id, game_center_achievement_localization_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_achievement_localization_response import GameCenterAchievementLocalizationResponse
from openapi_client.models.game_center_achievement_localization_update_request import GameCenterAchievementLocalizationUpdateRequest
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
    api_instance = openapi_client.GameCenterAchievementLocalizationsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_achievement_localization_update_request = openapi_client.GameCenterAchievementLocalizationUpdateRequest() # GameCenterAchievementLocalizationUpdateRequest | GameCenterAchievementLocalization representation

    try:
        api_response = api_instance.game_center_achievement_localizations_update_instance(id, game_center_achievement_localization_update_request)
        print("The response of GameCenterAchievementLocalizationsApi->game_center_achievement_localizations_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterAchievementLocalizationsApi->game_center_achievement_localizations_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_achievement_localization_update_request** | [**GameCenterAchievementLocalizationUpdateRequest**](GameCenterAchievementLocalizationUpdateRequest.md)| GameCenterAchievementLocalization representation | 

### Return type

[**GameCenterAchievementLocalizationResponse**](GameCenterAchievementLocalizationResponse.md)

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
**200** | Single GameCenterAchievementLocalization |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

