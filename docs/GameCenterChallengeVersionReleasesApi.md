# openapi_client.GameCenterChallengeVersionReleasesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_challenge_version_releases_create_instance**](GameCenterChallengeVersionReleasesApi.md#game_center_challenge_version_releases_create_instance) | **POST** /v1/gameCenterChallengeVersionReleases | 
[**game_center_challenge_version_releases_delete_instance**](GameCenterChallengeVersionReleasesApi.md#game_center_challenge_version_releases_delete_instance) | **DELETE** /v1/gameCenterChallengeVersionReleases/{id} | 
[**game_center_challenge_version_releases_get_instance**](GameCenterChallengeVersionReleasesApi.md#game_center_challenge_version_releases_get_instance) | **GET** /v1/gameCenterChallengeVersionReleases/{id} | 


# **game_center_challenge_version_releases_create_instance**
> GameCenterChallengeVersionReleaseResponse game_center_challenge_version_releases_create_instance(game_center_challenge_version_release_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_challenge_version_release_create_request import GameCenterChallengeVersionReleaseCreateRequest
from openapi_client.models.game_center_challenge_version_release_response import GameCenterChallengeVersionReleaseResponse
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
    api_instance = openapi_client.GameCenterChallengeVersionReleasesApi(api_client)
    game_center_challenge_version_release_create_request = openapi_client.GameCenterChallengeVersionReleaseCreateRequest() # GameCenterChallengeVersionReleaseCreateRequest | GameCenterChallengeVersionRelease representation

    try:
        api_response = api_instance.game_center_challenge_version_releases_create_instance(game_center_challenge_version_release_create_request)
        print("The response of GameCenterChallengeVersionReleasesApi->game_center_challenge_version_releases_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterChallengeVersionReleasesApi->game_center_challenge_version_releases_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_challenge_version_release_create_request** | [**GameCenterChallengeVersionReleaseCreateRequest**](GameCenterChallengeVersionReleaseCreateRequest.md)| GameCenterChallengeVersionRelease representation | 

### Return type

[**GameCenterChallengeVersionReleaseResponse**](GameCenterChallengeVersionReleaseResponse.md)

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
**201** | Single GameCenterChallengeVersionRelease |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_challenge_version_releases_delete_instance**
> game_center_challenge_version_releases_delete_instance(id)

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
    api_instance = openapi_client.GameCenterChallengeVersionReleasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.game_center_challenge_version_releases_delete_instance(id)
    except Exception as e:
        print("Exception when calling GameCenterChallengeVersionReleasesApi->game_center_challenge_version_releases_delete_instance: %s\n" % e)
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

# **game_center_challenge_version_releases_get_instance**
> GameCenterChallengeVersionReleaseResponse game_center_challenge_version_releases_get_instance(id, fields_game_center_challenge_version_releases=fields_game_center_challenge_version_releases, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_challenge_version_release_response import GameCenterChallengeVersionReleaseResponse
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
    api_instance = openapi_client.GameCenterChallengeVersionReleasesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_challenge_version_releases = ['fields_game_center_challenge_version_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterChallengeVersionReleases (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.game_center_challenge_version_releases_get_instance(id, fields_game_center_challenge_version_releases=fields_game_center_challenge_version_releases, include=include)
        print("The response of GameCenterChallengeVersionReleasesApi->game_center_challenge_version_releases_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterChallengeVersionReleasesApi->game_center_challenge_version_releases_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_challenge_version_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallengeVersionReleases | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**GameCenterChallengeVersionReleaseResponse**](GameCenterChallengeVersionReleaseResponse.md)

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
**200** | Single GameCenterChallengeVersionRelease |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

