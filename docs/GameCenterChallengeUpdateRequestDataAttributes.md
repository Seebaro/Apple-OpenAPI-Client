# GameCenterChallengeUpdateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | [optional] 
**allowed_durations** | **List[str]** |  | [optional] 
**archived** | **bool** |  | [optional] 
**repeatable** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_update_request_data_attributes import GameCenterChallengeUpdateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeUpdateRequestDataAttributes from a JSON string
game_center_challenge_update_request_data_attributes_instance = GameCenterChallengeUpdateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeUpdateRequestDataAttributes.to_json())

# convert the object into a dict
game_center_challenge_update_request_data_attributes_dict = game_center_challenge_update_request_data_attributes_instance.to_dict()
# create an instance of GameCenterChallengeUpdateRequestDataAttributes from a dict
game_center_challenge_update_request_data_attributes_from_dict = GameCenterChallengeUpdateRequestDataAttributes.from_dict(game_center_challenge_update_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


