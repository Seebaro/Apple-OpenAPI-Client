# GameCenterGroupRelationshipsGameCenterDetails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppRelationshipsGameCenterDetailData]**](AppRelationshipsGameCenterDetailData.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_group_relationships_game_center_details import GameCenterGroupRelationshipsGameCenterDetails

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterGroupRelationshipsGameCenterDetails from a JSON string
game_center_group_relationships_game_center_details_instance = GameCenterGroupRelationshipsGameCenterDetails.from_json(json)
# print the JSON string representation of the object
print(GameCenterGroupRelationshipsGameCenterDetails.to_json())

# convert the object into a dict
game_center_group_relationships_game_center_details_dict = game_center_group_relationships_game_center_details_instance.to_dict()
# create an instance of GameCenterGroupRelationshipsGameCenterDetails from a dict
game_center_group_relationships_game_center_details_from_dict = GameCenterGroupRelationshipsGameCenterDetails.from_dict(game_center_group_relationships_game_center_details_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


