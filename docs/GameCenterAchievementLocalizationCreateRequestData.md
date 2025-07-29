# GameCenterAchievementLocalizationCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterAchievementLocalizationCreateRequestDataAttributes**](GameCenterAchievementLocalizationCreateRequestDataAttributes.md) |  | 
**relationships** | [**GameCenterAchievementLocalizationCreateRequestDataRelationships**](GameCenterAchievementLocalizationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.game_center_achievement_localization_create_request_data import GameCenterAchievementLocalizationCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementLocalizationCreateRequestData from a JSON string
game_center_achievement_localization_create_request_data_instance = GameCenterAchievementLocalizationCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementLocalizationCreateRequestData.to_json())

# convert the object into a dict
game_center_achievement_localization_create_request_data_dict = game_center_achievement_localization_create_request_data_instance.to_dict()
# create an instance of GameCenterAchievementLocalizationCreateRequestData from a dict
game_center_achievement_localization_create_request_data_from_dict = GameCenterAchievementLocalizationCreateRequestData.from_dict(game_center_achievement_localization_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


