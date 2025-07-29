# GameCenterChallengeUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterChallengeUpdateRequestDataAttributes**](GameCenterChallengeUpdateRequestDataAttributes.md) |  | [optional] 
**relationships** | [**GameCenterChallengeUpdateRequestDataRelationships**](GameCenterChallengeUpdateRequestDataRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_update_request_data import GameCenterChallengeUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeUpdateRequestData from a JSON string
game_center_challenge_update_request_data_instance = GameCenterChallengeUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeUpdateRequestData.to_json())

# convert the object into a dict
game_center_challenge_update_request_data_dict = game_center_challenge_update_request_data_instance.to_dict()
# create an instance of GameCenterChallengeUpdateRequestData from a dict
game_center_challenge_update_request_data_from_dict = GameCenterChallengeUpdateRequestData.from_dict(game_center_challenge_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


