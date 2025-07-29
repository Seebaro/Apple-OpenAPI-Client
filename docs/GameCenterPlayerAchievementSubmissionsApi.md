# openapi_client.GameCenterPlayerAchievementSubmissionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**game_center_player_achievement_submissions_create_instance**](GameCenterPlayerAchievementSubmissionsApi.md#game_center_player_achievement_submissions_create_instance) | **POST** /v1/gameCenterPlayerAchievementSubmissions | 


# **game_center_player_achievement_submissions_create_instance**
> GameCenterPlayerAchievementSubmissionResponse game_center_player_achievement_submissions_create_instance(game_center_player_achievement_submission_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.game_center_player_achievement_submission_create_request import GameCenterPlayerAchievementSubmissionCreateRequest
from openapi_client.models.game_center_player_achievement_submission_response import GameCenterPlayerAchievementSubmissionResponse
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
    api_instance = openapi_client.GameCenterPlayerAchievementSubmissionsApi(api_client)
    game_center_player_achievement_submission_create_request = openapi_client.GameCenterPlayerAchievementSubmissionCreateRequest() # GameCenterPlayerAchievementSubmissionCreateRequest | GameCenterPlayerAchievementSubmission representation

    try:
        api_response = api_instance.game_center_player_achievement_submissions_create_instance(game_center_player_achievement_submission_create_request)
        print("The response of GameCenterPlayerAchievementSubmissionsApi->game_center_player_achievement_submissions_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GameCenterPlayerAchievementSubmissionsApi->game_center_player_achievement_submissions_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **game_center_player_achievement_submission_create_request** | [**GameCenterPlayerAchievementSubmissionCreateRequest**](GameCenterPlayerAchievementSubmissionCreateRequest.md)| GameCenterPlayerAchievementSubmission representation | 

### Return type

[**GameCenterPlayerAchievementSubmissionResponse**](GameCenterPlayerAchievementSubmissionResponse.md)

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
**201** | Single GameCenterPlayerAchievementSubmission |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

