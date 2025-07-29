# GameCenterAchievementReleaseCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**game_center_detail** | [**GameCenterAchievementReleaseCreateRequestDataRelationshipsGameCenterDetail**](GameCenterAchievementReleaseCreateRequestDataRelationshipsGameCenterDetail.md) |  | 
**game_center_achievement** | [**GameCenterAchievementLocalizationCreateRequestDataRelationshipsGameCenterAchievement**](GameCenterAchievementLocalizationCreateRequestDataRelationshipsGameCenterAchievement.md) |  | 

## Example

```python
from openapi_client.models.game_center_achievement_release_create_request_data_relationships import GameCenterAchievementReleaseCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementReleaseCreateRequestDataRelationships from a JSON string
game_center_achievement_release_create_request_data_relationships_instance = GameCenterAchievementReleaseCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementReleaseCreateRequestDataRelationships.to_json())

# convert the object into a dict
game_center_achievement_release_create_request_data_relationships_dict = game_center_achievement_release_create_request_data_relationships_instance.to_dict()
# create an instance of GameCenterAchievementReleaseCreateRequestDataRelationships from a dict
game_center_achievement_release_create_request_data_relationships_from_dict = GameCenterAchievementReleaseCreateRequestDataRelationships.from_dict(game_center_achievement_release_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


