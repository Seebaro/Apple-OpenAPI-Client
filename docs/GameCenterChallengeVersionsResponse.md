# GameCenterChallengeVersionsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterChallengeVersion]**](GameCenterChallengeVersion.md) |  | 
**included** | [**List[GameCenterChallengeVersionsResponseIncludedInner]**](GameCenterChallengeVersionsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_versions_response import GameCenterChallengeVersionsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeVersionsResponse from a JSON string
game_center_challenge_versions_response_instance = GameCenterChallengeVersionsResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeVersionsResponse.to_json())

# convert the object into a dict
game_center_challenge_versions_response_dict = game_center_challenge_versions_response_instance.to_dict()
# create an instance of GameCenterChallengeVersionsResponse from a dict
game_center_challenge_versions_response_from_dict = GameCenterChallengeVersionsResponse.from_dict(game_center_challenge_versions_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


