# GameCenterAchievementGroupAchievementLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterAchievementLocalizationRelationshipsGameCenterAchievementData**](GameCenterAchievementLocalizationRelationshipsGameCenterAchievementData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_achievement_group_achievement_linkage_response import GameCenterAchievementGroupAchievementLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementGroupAchievementLinkageResponse from a JSON string
game_center_achievement_group_achievement_linkage_response_instance = GameCenterAchievementGroupAchievementLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementGroupAchievementLinkageResponse.to_json())

# convert the object into a dict
game_center_achievement_group_achievement_linkage_response_dict = game_center_achievement_group_achievement_linkage_response_instance.to_dict()
# create an instance of GameCenterAchievementGroupAchievementLinkageResponse from a dict
game_center_achievement_group_achievement_linkage_response_from_dict = GameCenterAchievementGroupAchievementLinkageResponse.from_dict(game_center_achievement_group_achievement_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


