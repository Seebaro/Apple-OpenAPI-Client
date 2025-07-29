# GameCenterDetailRelationshipsGameCenterActivities


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[GameCenterAchievementRelationshipsActivityData]**](GameCenterAchievementRelationshipsActivityData.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_detail_relationships_game_center_activities import GameCenterDetailRelationshipsGameCenterActivities

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailRelationshipsGameCenterActivities from a JSON string
game_center_detail_relationships_game_center_activities_instance = GameCenterDetailRelationshipsGameCenterActivities.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailRelationshipsGameCenterActivities.to_json())

# convert the object into a dict
game_center_detail_relationships_game_center_activities_dict = game_center_detail_relationships_game_center_activities_instance.to_dict()
# create an instance of GameCenterDetailRelationshipsGameCenterActivities from a dict
game_center_detail_relationships_game_center_activities_from_dict = GameCenterDetailRelationshipsGameCenterActivities.from_dict(game_center_detail_relationships_game_center_activities_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


