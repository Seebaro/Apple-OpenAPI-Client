# GameCenterAchievementCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterAchievementCreateRequestDataAttributes**](GameCenterAchievementCreateRequestDataAttributes.md) |  | 
**relationships** | [**GameCenterAchievementCreateRequestDataRelationships**](GameCenterAchievementCreateRequestDataRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievement_create_request_data import GameCenterAchievementCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementCreateRequestData from a JSON string
game_center_achievement_create_request_data_instance = GameCenterAchievementCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementCreateRequestData.to_json())

# convert the object into a dict
game_center_achievement_create_request_data_dict = game_center_achievement_create_request_data_instance.to_dict()
# create an instance of GameCenterAchievementCreateRequestData from a dict
game_center_achievement_create_request_data_from_dict = GameCenterAchievementCreateRequestData.from_dict(game_center_achievement_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


