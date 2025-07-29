# GameCenterChallengeLocalizationCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterActivityLocalizationCreateRequestDataAttributes**](GameCenterActivityLocalizationCreateRequestDataAttributes.md) |  | 
**relationships** | [**GameCenterChallengeLocalizationCreateRequestDataRelationships**](GameCenterChallengeLocalizationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.game_center_challenge_localization_create_request_data import GameCenterChallengeLocalizationCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeLocalizationCreateRequestData from a JSON string
game_center_challenge_localization_create_request_data_instance = GameCenterChallengeLocalizationCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeLocalizationCreateRequestData.to_json())

# convert the object into a dict
game_center_challenge_localization_create_request_data_dict = game_center_challenge_localization_create_request_data_instance.to_dict()
# create an instance of GameCenterChallengeLocalizationCreateRequestData from a dict
game_center_challenge_localization_create_request_data_from_dict = GameCenterChallengeLocalizationCreateRequestData.from_dict(game_center_challenge_localization_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


