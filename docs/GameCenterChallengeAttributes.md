# GameCenterChallengeAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | [optional] 
**vendor_identifier** | **str** |  | [optional] 
**allowed_durations** | **List[str]** |  | [optional] 
**archived** | **bool** |  | [optional] 
**challenge_type** | **str** |  | [optional] 
**repeatable** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_attributes import GameCenterChallengeAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeAttributes from a JSON string
game_center_challenge_attributes_instance = GameCenterChallengeAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeAttributes.to_json())

# convert the object into a dict
game_center_challenge_attributes_dict = game_center_challenge_attributes_instance.to_dict()
# create an instance of GameCenterChallengeAttributes from a dict
game_center_challenge_attributes_from_dict = GameCenterChallengeAttributes.from_dict(game_center_challenge_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


