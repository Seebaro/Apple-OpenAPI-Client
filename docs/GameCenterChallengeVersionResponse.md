# GameCenterChallengeVersionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterChallengeVersion**](GameCenterChallengeVersion.md) |  | 
**included** | [**List[GameCenterChallengeVersionsResponseIncludedInner]**](GameCenterChallengeVersionsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_challenge_version_response import GameCenterChallengeVersionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeVersionResponse from a JSON string
game_center_challenge_version_response_instance = GameCenterChallengeVersionResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeVersionResponse.to_json())

# convert the object into a dict
game_center_challenge_version_response_dict = game_center_challenge_version_response_instance.to_dict()
# create an instance of GameCenterChallengeVersionResponse from a dict
game_center_challenge_version_response_from_dict = GameCenterChallengeVersionResponse.from_dict(game_center_challenge_version_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


