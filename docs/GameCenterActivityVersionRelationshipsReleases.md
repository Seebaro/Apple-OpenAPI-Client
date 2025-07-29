# GameCenterActivityVersionRelationshipsReleases


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[GameCenterActivityVersionRelationshipsReleasesDataInner]**](GameCenterActivityVersionRelationshipsReleasesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_activity_version_relationships_releases import GameCenterActivityVersionRelationshipsReleases

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityVersionRelationshipsReleases from a JSON string
game_center_activity_version_relationships_releases_instance = GameCenterActivityVersionRelationshipsReleases.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityVersionRelationshipsReleases.to_json())

# convert the object into a dict
game_center_activity_version_relationships_releases_dict = game_center_activity_version_relationships_releases_instance.to_dict()
# create an instance of GameCenterActivityVersionRelationshipsReleases from a dict
game_center_activity_version_relationships_releases_from_dict = GameCenterActivityVersionRelationshipsReleases.from_dict(game_center_activity_version_relationships_releases_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


