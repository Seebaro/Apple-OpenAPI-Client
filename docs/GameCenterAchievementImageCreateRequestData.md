# GameCenterAchievementImageCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppClipAdvancedExperienceImageCreateRequestDataAttributes**](AppClipAdvancedExperienceImageCreateRequestDataAttributes.md) |  | 
**relationships** | [**GameCenterAchievementImageCreateRequestDataRelationships**](GameCenterAchievementImageCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.game_center_achievement_image_create_request_data import GameCenterAchievementImageCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementImageCreateRequestData from a JSON string
game_center_achievement_image_create_request_data_instance = GameCenterAchievementImageCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementImageCreateRequestData.to_json())

# convert the object into a dict
game_center_achievement_image_create_request_data_dict = game_center_achievement_image_create_request_data_instance.to_dict()
# create an instance of GameCenterAchievementImageCreateRequestData from a dict
game_center_achievement_image_create_request_data_from_dict = GameCenterAchievementImageCreateRequestData.from_dict(game_center_achievement_image_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


