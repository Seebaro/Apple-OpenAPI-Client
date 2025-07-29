# GameCenterChallengeVersionReleasesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterChallengeVersionRelease]**](GameCenterChallengeVersionRelease.md) |  | 
**included** | [**List[GameCenterChallengeVersion]**](GameCenterChallengeVersion.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_version_releases_response import GameCenterChallengeVersionReleasesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeVersionReleasesResponse from a JSON string
game_center_challenge_version_releases_response_instance = GameCenterChallengeVersionReleasesResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeVersionReleasesResponse.to_json())

# convert the object into a dict
game_center_challenge_version_releases_response_dict = game_center_challenge_version_releases_response_instance.to_dict()
# create an instance of GameCenterChallengeVersionReleasesResponse from a dict
game_center_challenge_version_releases_response_from_dict = GameCenterChallengeVersionReleasesResponse.from_dict(game_center_challenge_version_releases_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


