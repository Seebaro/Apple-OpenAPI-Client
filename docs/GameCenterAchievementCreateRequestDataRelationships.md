# GameCenterAchievementCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**game_center_detail** | [**GameCenterAchievementReleaseRelationshipsGameCenterDetail**](GameCenterAchievementReleaseRelationshipsGameCenterDetail.md) |  | [optional] 
**game_center_group** | [**GameCenterAchievementRelationshipsGameCenterGroup**](GameCenterAchievementRelationshipsGameCenterGroup.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievement_create_request_data_relationships import GameCenterAchievementCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementCreateRequestDataRelationships from a JSON string
game_center_achievement_create_request_data_relationships_instance = GameCenterAchievementCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementCreateRequestDataRelationships.to_json())

# convert the object into a dict
game_center_achievement_create_request_data_relationships_dict = game_center_achievement_create_request_data_relationships_instance.to_dict()
# create an instance of GameCenterAchievementCreateRequestDataRelationships from a dict
game_center_achievement_create_request_data_relationships_from_dict = GameCenterAchievementCreateRequestDataRelationships.from_dict(game_center_achievement_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


