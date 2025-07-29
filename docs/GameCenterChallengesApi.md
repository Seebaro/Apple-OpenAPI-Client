# openapi_client.GameCenterChallengesApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_challenges_create_instance**](GameCenterChallengesApi.md#game_center_challenges_create_instance) | **POST** /v1/gameCenterChallenges | 
[**game_center_challenges_delete_instance**](GameCenterChallengesApi.md#game_center_challenges_delete_instance) | **DELETE** /v1/gameCenterChallenges/{id} | 
[**game_center_challenges_get_instance**](GameCenterChallengesApi.md#game_center_challenges_get_instance) | **GET** /v1/gameCenterChallenges/{id} | 
[**game_center_challenges_leaderboard_update_to_one_relationship**](GameCenterChallengesApi.md#game_center_challenges_leaderboard_update_to_one_relationship) | **PATCH** /v1/gameCenterChallenges/{id}/relationships/leaderboard | 
[**game_center_challenges_update_instance**](GameCenterChallengesApi.md#game_center_challenges_update_instance) | **PATCH** /v1/gameCenterChallenges/{id} | 
[**game_center_challenges_versions_get_to_many_related**](GameCenterChallengesApi.md#game_center_challenges_versions_get_to_many_related) | **GET** /v1/gameCenterChallenges/{id}/versions | 
[**game_center_challenges_versions_get_to_many_relationship**](GameCenterChallengesApi.md#game_center_challenges_versions_get_to_many_relationship) | **GET** /v1/gameCenterChallenges/{id}/relationships/versions | 


# **game_center_challenges_create_instance**
> GameCenterChallengeResponse game_center_challenges_create_instance(game_center_challenge_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_challenge_create_request import GameCenterChallengeCreateRequest
from openapi_client.models.game_center_challenge_response import GameCenterChallengeResponse
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
    api_instance = openapi_client.GameCenterChallengesApi(api_client)
    game_center_challenge_create_request = openapi_client.GameCenterChallengeCreateRequest() # GameCenterChallengeCreateRequest | GameCenterChallenge representation

    try:
        api_response = api_instance.game_center_challenges_create_instance(game_center_challenge_create_request)
        print("The response of GameCenterChallengesApi->game_center_challenges_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterChallengesApi->game_center_challenges_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_challenge_create_request** | [**GameCenterChallengeCreateRequest**](GameCenterChallengeCreateRequest.md)| GameCenterChallenge representation | 

### Return type

[**GameCenterChallengeResponse**](GameCenterChallengeResponse.md)

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
**201** | Single GameCenterChallenge |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_challenges_delete_instance**
> game_center_challenges_delete_instance(id)

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
    api_instance = openapi_client.GameCenterChallengesApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.game_center_challenges_delete_instance(id)
    except Exception as e:
        print("Exception when calling GameCenterChallengesApi->game_center_challenges_delete_instance: %s\n" % e)
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

# **game_center_challenges_get_instance**
> GameCenterChallengeResponse game_center_challenges_get_instance(id, fields_game_center_challenges=fields_game_center_challenges, fields_game_center_challenge_versions=fields_game_center_challenge_versions, include=include, limit_versions=limit_versions)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_challenge_response import GameCenterChallengeResponse
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
    api_instance = openapi_client.GameCenterChallengesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_challenges = ['fields_game_center_challenges_example'] # List[str] | the fields to include for returned resources of type gameCenterChallenges (optional)
    fields_game_center_challenge_versions = ['fields_game_center_challenge_versions_example'] # List[str] | the fields to include for returned resources of type gameCenterChallengeVersions (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_versions = 56 # int | maximum number of related versions returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_challenges_get_instance(id, fields_game_center_challenges=fields_game_center_challenges, fields_game_center_challenge_versions=fields_game_center_challenge_versions, include=include, limit_versions=limit_versions)
        print("The response of GameCenterChallengesApi->game_center_challenges_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterChallengesApi->game_center_challenges_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_challenges** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallenges | [optional] 
 **fields_game_center_challenge_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallengeVersions | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_versions** | **int**| maximum number of related versions returned (when they are included) | [optional] 

### Return type

[**GameCenterChallengeResponse**](GameCenterChallengeResponse.md)

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
**200** | Single GameCenterChallenge |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_challenges_leaderboard_update_to_one_relationship**
> game_center_challenges_leaderboard_update_to_one_relationship(id, game_center_challenge_leaderboard_linkage_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_challenge_leaderboard_linkage_request import GameCenterChallengeLeaderboardLinkageRequest
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
    api_instance = openapi_client.GameCenterChallengesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_challenge_leaderboard_linkage_request = openapi_client.GameCenterChallengeLeaderboardLinkageRequest() # GameCenterChallengeLeaderboardLinkageRequest | Related linkage

    try:
        api_instance.game_center_challenges_leaderboard_update_to_one_relationship(id, game_center_challenge_leaderboard_linkage_request)
    except Exception as e:
        print("Exception when calling GameCenterChallengesApi->game_center_challenges_leaderboard_update_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_challenge_leaderboard_linkage_request** | [**GameCenterChallengeLeaderboardLinkageRequest**](GameCenterChallengeLeaderboardLinkageRequest.md)| Related linkage | 

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**409** | Request entity error(s) |  -  |
**204** | Success (no content) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_challenges_update_instance**
> GameCenterChallengeResponse game_center_challenges_update_instance(id, game_center_challenge_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_challenge_response import GameCenterChallengeResponse
from openapi_client.models.game_center_challenge_update_request import GameCenterChallengeUpdateRequest
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
    api_instance = openapi_client.GameCenterChallengesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    game_center_challenge_update_request = openapi_client.GameCenterChallengeUpdateRequest() # GameCenterChallengeUpdateRequest | GameCenterChallenge representation

    try:
        api_response = api_instance.game_center_challenges_update_instance(id, game_center_challenge_update_request)
        print("The response of GameCenterChallengesApi->game_center_challenges_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterChallengesApi->game_center_challenges_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **game_center_challenge_update_request** | [**GameCenterChallengeUpdateRequest**](GameCenterChallengeUpdateRequest.md)| GameCenterChallenge representation | 

### Return type

[**GameCenterChallengeResponse**](GameCenterChallengeResponse.md)

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
**200** | Single GameCenterChallenge |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_challenges_versions_get_to_many_related**
> GameCenterChallengeVersionsResponse game_center_challenges_versions_get_to_many_related(id, fields_game_center_challenge_versions=fields_game_center_challenge_versions, fields_game_center_challenges=fields_game_center_challenges, fields_game_center_challenge_localizations=fields_game_center_challenge_localizations, fields_game_center_challenge_version_releases=fields_game_center_challenge_version_releases, fields_game_center_challenge_images=fields_game_center_challenge_images, limit=limit, include=include, limit_localizations=limit_localizations, limit_releases=limit_releases)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_challenge_versions_response import GameCenterChallengeVersionsResponse
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
    api_instance = openapi_client.GameCenterChallengesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_game_center_challenge_versions = ['fields_game_center_challenge_versions_example'] # List[str] | the fields to include for returned resources of type gameCenterChallengeVersions (optional)
    fields_game_center_challenges = ['fields_game_center_challenges_example'] # List[str] | the fields to include for returned resources of type gameCenterChallenges (optional)
    fields_game_center_challenge_localizations = ['fields_game_center_challenge_localizations_example'] # List[str] | the fields to include for returned resources of type gameCenterChallengeLocalizations (optional)
    fields_game_center_challenge_version_releases = ['fields_game_center_challenge_version_releases_example'] # List[str] | the fields to include for returned resources of type gameCenterChallengeVersionReleases (optional)
    fields_game_center_challenge_images = ['fields_game_center_challenge_images_example'] # List[str] | the fields to include for returned resources of type gameCenterChallengeImages (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_localizations = 56 # int | maximum number of related localizations returned (when they are included) (optional)
    limit_releases = 56 # int | maximum number of related releases returned (when they are included) (optional)

    try:
        api_response = api_instance.game_center_challenges_versions_get_to_many_related(id, fields_game_center_challenge_versions=fields_game_center_challenge_versions, fields_game_center_challenges=fields_game_center_challenges, fields_game_center_challenge_localizations=fields_game_center_challenge_localizations, fields_game_center_challenge_version_releases=fields_game_center_challenge_version_releases, fields_game_center_challenge_images=fields_game_center_challenge_images, limit=limit, include=include, limit_localizations=limit_localizations, limit_releases=limit_releases)
        print("The response of GameCenterChallengesApi->game_center_challenges_versions_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterChallengesApi->game_center_challenges_versions_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_game_center_challenge_versions** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallengeVersions | [optional] 
 **fields_game_center_challenges** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallenges | [optional] 
 **fields_game_center_challenge_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallengeLocalizations | [optional] 
 **fields_game_center_challenge_version_releases** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallengeVersionReleases | [optional] 
 **fields_game_center_challenge_images** | [**List[str]**](str.md)| the fields to include for returned resources of type gameCenterChallengeImages | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_localizations** | **int**| maximum number of related localizations returned (when they are included) | [optional] 
 **limit_releases** | **int**| maximum number of related releases returned (when they are included) | [optional] 

### Return type

[**GameCenterChallengeVersionsResponse**](GameCenterChallengeVersionsResponse.md)

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
**200** | List of GameCenterChallengeVersions |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **game_center_challenges_versions_get_to_many_relationship**
> GameCenterChallengeVersionsLinkagesResponse game_center_challenges_versions_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_challenge_versions_linkages_response import GameCenterChallengeVersionsLinkagesResponse
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
    api_instance = openapi_client.GameCenterChallengesApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.game_center_challenges_versions_get_to_many_relationship(id, limit=limit)
        print("The response of GameCenterChallengesApi->game_center_challenges_versions_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterChallengesApi->game_center_challenges_versions_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**GameCenterChallengeVersionsLinkagesResponse**](GameCenterChallengeVersionsLinkagesResponse.md)

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

