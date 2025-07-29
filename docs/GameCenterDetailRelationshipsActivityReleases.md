# GameCenterDetailRelationshipsActivityReleases


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[GameCenterActivityVersionRelationshipsReleasesDataInner]**](GameCenterActivityVersionRelationshipsReleasesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_detail_relationships_activity_releases import GameCenterDetailRelationshipsActivityReleases

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailRelationshipsActivityReleases from a JSON string
game_center_detail_relationships_activity_releases_instance = GameCenterDetailRelationshipsActivityReleases.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailRelationshipsActivityReleases.to_json())

# convert the object into a dict
game_center_detail_relationships_activity_releases_dict = game_center_detail_relationships_activity_releases_instance.to_dict()
# create an instance of GameCenterDetailRelationshipsActivityReleases from a dict
game_center_detail_relationships_activity_releases_from_dict = GameCenterDetailRelationshipsActivityReleases.from_dict(game_center_detail_relationships_activity_releases_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


