# GameCenterChallengeCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterChallengeCreateRequestDataAttributes**](GameCenterChallengeCreateRequestDataAttributes.md) |  | 
**relationships** | [**GameCenterChallengeCreateRequestDataRelationships**](GameCenterChallengeCreateRequestDataRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_create_request_data import GameCenterChallengeCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeCreateRequestData from a JSON string
game_center_challenge_create_request_data_instance = GameCenterChallengeCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeCreateRequestData.to_json())

# convert the object into a dict
game_center_challenge_create_request_data_dict = game_center_challenge_create_request_data_instance.to_dict()
# create an instance of GameCenterChallengeCreateRequestData from a dict
game_center_challenge_create_request_data_from_dict = GameCenterChallengeCreateRequestData.from_dict(game_center_challenge_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


