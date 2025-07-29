# GameCenterActivityRelationshipsVersions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[GameCenterActivityRelationshipsVersionsDataInner]**](GameCenterActivityRelationshipsVersionsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_activity_relationships_versions import GameCenterActivityRelationshipsVersions

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityRelationshipsVersions from a JSON string
game_center_activity_relationships_versions_instance = GameCenterActivityRelationshipsVersions.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityRelationshipsVersions.to_json())

# convert the object into a dict
game_center_activity_relationships_versions_dict = game_center_activity_relationships_versions_instance.to_dict()
# create an instance of GameCenterActivityRelationshipsVersions from a dict
game_center_activity_relationships_versions_from_dict = GameCenterActivityRelationshipsVersions.from_dict(game_center_activity_relationships_versions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


