# GameCenterChallengeVersionAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**version** | **int** |  | [optional] 
**state** | [**GameCenterVersionState**](GameCenterVersionState.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_version_attributes import GameCenterChallengeVersionAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeVersionAttributes from a JSON string
game_center_challenge_version_attributes_instance = GameCenterChallengeVersionAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeVersionAttributes.to_json())

# convert the object into a dict
game_center_challenge_version_attributes_dict = game_center_challenge_version_attributes_instance.to_dict()
# create an instance of GameCenterChallengeVersionAttributes from a dict
game_center_challenge_version_attributes_from_dict = GameCenterChallengeVersionAttributes.from_dict(game_center_challenge_version_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


