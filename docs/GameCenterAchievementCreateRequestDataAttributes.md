# GameCenterAchievementCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | 
**vendor_identifier** | **str** |  | 
**points** | **int** |  | 
**show_before_earned** | **bool** |  | 
**repeatable** | **bool** |  | 
**activity_properties** | **Dict[str, str]** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievement_create_request_data_attributes import GameCenterAchievementCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementCreateRequestDataAttributes from a JSON string
game_center_achievement_create_request_data_attributes_instance = GameCenterAchievementCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementCreateRequestDataAttributes.to_json())

# convert the object into a dict
game_center_achievement_create_request_data_attributes_dict = game_center_achievement_create_request_data_attributes_instance.to_dict()
# create an instance of GameCenterAchievementCreateRequestDataAttributes from a dict
game_center_achievement_create_request_data_attributes_from_dict = GameCenterAchievementCreateRequestDataAttributes.from_dict(game_center_achievement_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


