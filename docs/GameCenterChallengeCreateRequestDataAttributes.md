# GameCenterChallengeCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | 
**vendor_identifier** | **str** |  | 
**allowed_durations** | **List[str]** |  | [optional] 
**challenge_type** | **str** |  | 
**repeatable** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_create_request_data_attributes import GameCenterChallengeCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeCreateRequestDataAttributes from a JSON string
game_center_challenge_create_request_data_attributes_instance = GameCenterChallengeCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeCreateRequestDataAttributes.to_json())

# convert the object into a dict
game_center_challenge_create_request_data_attributes_dict = game_center_challenge_create_request_data_attributes_instance.to_dict()
# create an instance of GameCenterChallengeCreateRequestDataAttributes from a dict
game_center_challenge_create_request_data_attributes_from_dict = GameCenterChallengeCreateRequestDataAttributes.from_dict(game_center_challenge_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


