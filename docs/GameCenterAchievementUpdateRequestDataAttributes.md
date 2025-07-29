# GameCenterAchievementUpdateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | [optional] 
**points** | **int** |  | [optional] 
**show_before_earned** | **bool** |  | [optional] 
**repeatable** | **bool** |  | [optional] 
**archived** | **bool** |  | [optional] 
**activity_properties** | **Dict[str, str]** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievement_update_request_data_attributes import GameCenterAchievementUpdateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementUpdateRequestDataAttributes from a JSON string
game_center_achievement_update_request_data_attributes_instance = GameCenterAchievementUpdateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementUpdateRequestDataAttributes.to_json())

# convert the object into a dict
game_center_achievement_update_request_data_attributes_dict = game_center_achievement_update_request_data_attributes_instance.to_dict()
# create an instance of GameCenterAchievementUpdateRequestDataAttributes from a dict
game_center_achievement_update_request_data_attributes_from_dict = GameCenterAchievementUpdateRequestDataAttributes.from_dict(game_center_achievement_update_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


