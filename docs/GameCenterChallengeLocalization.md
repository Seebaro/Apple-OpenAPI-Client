# GameCenterChallengeLocalization


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterActivityLocalizationAttributes**](GameCenterActivityLocalizationAttributes.md) |  | [optional] 
**relationships** | [**GameCenterChallengeLocalizationRelationships**](GameCenterChallengeLocalizationRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_localization import GameCenterChallengeLocalization

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeLocalization from a JSON string
game_center_challenge_localization_instance = GameCenterChallengeLocalization.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeLocalization.to_json())

# convert the object into a dict
game_center_challenge_localization_dict = game_center_challenge_localization_instance.to_dict()
# create an instance of GameCenterChallengeLocalization from a dict
game_center_challenge_localization_from_dict = GameCenterChallengeLocalization.from_dict(game_center_challenge_localization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


