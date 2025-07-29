# GameCenterChallengeVersionCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**GameCenterChallengeVersionCreateRequestDataRelationships**](GameCenterChallengeVersionCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.game_center_challenge_version_create_request_data import GameCenterChallengeVersionCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeVersionCreateRequestData from a JSON string
game_center_challenge_version_create_request_data_instance = GameCenterChallengeVersionCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeVersionCreateRequestData.to_json())

# convert the object into a dict
game_center_challenge_version_create_request_data_dict = game_center_challenge_version_create_request_data_instance.to_dict()
# create an instance of GameCenterChallengeVersionCreateRequestData from a dict
game_center_challenge_version_create_request_data_from_dict = GameCenterChallengeVersionCreateRequestData.from_dict(game_center_challenge_version_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


