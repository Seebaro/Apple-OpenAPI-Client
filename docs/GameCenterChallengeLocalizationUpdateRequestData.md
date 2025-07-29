# GameCenterChallengeLocalizationUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterActivityLocalizationUpdateRequestDataAttributes**](GameCenterActivityLocalizationUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_localization_update_request_data import GameCenterChallengeLocalizationUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeLocalizationUpdateRequestData from a JSON string
game_center_challenge_localization_update_request_data_instance = GameCenterChallengeLocalizationUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeLocalizationUpdateRequestData.to_json())

# convert the object into a dict
game_center_challenge_localization_update_request_data_dict = game_center_challenge_localization_update_request_data_instance.to_dict()
# create an instance of GameCenterChallengeLocalizationUpdateRequestData from a dict
game_center_challenge_localization_update_request_data_from_dict = GameCenterChallengeLocalizationUpdateRequestData.from_dict(game_center_challenge_localization_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


