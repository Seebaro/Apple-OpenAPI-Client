# GameCenterDetailRelationshipsGameCenterGroup


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**data** | [**GameCenterAchievementRelationshipsGameCenterGroupData**](GameCenterAchievementRelationshipsGameCenterGroupData.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_detail_relationships_game_center_group import GameCenterDetailRelationshipsGameCenterGroup

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailRelationshipsGameCenterGroup from a JSON string
game_center_detail_relationships_game_center_group_instance = GameCenterDetailRelationshipsGameCenterGroup.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailRelationshipsGameCenterGroup.to_json())

# convert the object into a dict
game_center_detail_relationships_game_center_group_dict = game_center_detail_relationships_game_center_group_instance.to_dict()
# create an instance of GameCenterDetailRelationshipsGameCenterGroup from a dict
game_center_detail_relationships_game_center_group_from_dict = GameCenterDetailRelationshipsGameCenterGroup.from_dict(game_center_detail_relationships_game_center_group_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


