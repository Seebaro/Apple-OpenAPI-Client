# GameCenterAppVersionRelationshipsCompatibilityVersions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppStoreVersionRelationshipsGameCenterAppVersionData]**](AppStoreVersionRelationshipsGameCenterAppVersionData.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_app_version_relationships_compatibility_versions import GameCenterAppVersionRelationshipsCompatibilityVersions

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAppVersionRelationshipsCompatibilityVersions from a JSON string
game_center_app_version_relationships_compatibility_versions_instance = GameCenterAppVersionRelationshipsCompatibilityVersions.from_json(json)
# print the JSON string representation of the object
print(GameCenterAppVersionRelationshipsCompatibilityVersions.to_json())

# convert the object into a dict
game_center_app_version_relationships_compatibility_versions_dict = game_center_app_version_relationships_compatibility_versions_instance.to_dict()
# create an instance of GameCenterAppVersionRelationshipsCompatibilityVersions from a dict
game_center_app_version_relationships_compatibility_versions_from_dict = GameCenterAppVersionRelationshipsCompatibilityVersions.from_dict(game_center_app_version_relationships_compatibility_versions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


