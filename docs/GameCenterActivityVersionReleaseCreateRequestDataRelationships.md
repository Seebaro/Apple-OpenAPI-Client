# GameCenterActivityVersionReleaseCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**game_center_detail** | [**GameCenterAchievementReleaseCreateRequestDataRelationshipsGameCenterDetail**](GameCenterAchievementReleaseCreateRequestDataRelationshipsGameCenterDetail.md) |  | 
**version** | [**GameCenterActivityLocalizationCreateRequestDataRelationshipsVersion**](GameCenterActivityLocalizationCreateRequestDataRelationshipsVersion.md) |  | 

## Example

```python
from openapi_client.models.game_center_activity_version_release_create_request_data_relationships import GameCenterActivityVersionReleaseCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityVersionReleaseCreateRequestDataRelationships from a JSON string
game_center_activity_version_release_create_request_data_relationships_instance = GameCenterActivityVersionReleaseCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityVersionReleaseCreateRequestDataRelationships.to_json())

# convert the object into a dict
game_center_activity_version_release_create_request_data_relationships_dict = game_center_activity_version_release_create_request_data_relationships_instance.to_dict()
# create an instance of GameCenterActivityVersionReleaseCreateRequestDataRelationships from a dict
game_center_activity_version_release_create_request_data_relationships_from_dict = GameCenterActivityVersionReleaseCreateRequestDataRelationships.from_dict(game_center_activity_version_release_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


