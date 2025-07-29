# GameCenterAppVersionRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**compatibility_versions** | [**GameCenterAppVersionRelationshipsCompatibilityVersions**](GameCenterAppVersionRelationshipsCompatibilityVersions.md) |  | [optional] 
**app_store_version** | [**AppClipDefaultExperienceRelationshipsReleaseWithAppStoreVersion**](AppClipDefaultExperienceRelationshipsReleaseWithAppStoreVersion.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_app_version_relationships import GameCenterAppVersionRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAppVersionRelationships from a JSON string
game_center_app_version_relationships_instance = GameCenterAppVersionRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterAppVersionRelationships.to_json())

# convert the object into a dict
game_center_app_version_relationships_dict = game_center_app_version_relationships_instance.to_dict()
# create an instance of GameCenterAppVersionRelationships from a dict
game_center_app_version_relationships_from_dict = GameCenterAppVersionRelationships.from_dict(game_center_app_version_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


