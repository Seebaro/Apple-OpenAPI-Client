# GameCenterAchievementAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | [optional] 
**vendor_identifier** | **str** |  | [optional] 
**points** | **int** |  | [optional] 
**show_before_earned** | **bool** |  | [optional] 
**repeatable** | **bool** |  | [optional] 
**archived** | **bool** |  | [optional] 
**activity_properties** | **Dict[str, str]** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievement_attributes import GameCenterAchievementAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementAttributes from a JSON string
game_center_achievement_attributes_instance = GameCenterAchievementAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementAttributes.to_json())

# convert the object into a dict
game_center_achievement_attributes_dict = game_center_achievement_attributes_instance.to_dict()
# create an instance of GameCenterAchievementAttributes from a dict
game_center_achievement_attributes_from_dict = GameCenterAchievementAttributes.from_dict(game_center_achievement_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


