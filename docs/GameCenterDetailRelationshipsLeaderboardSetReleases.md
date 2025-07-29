# GameCenterDetailRelationshipsLeaderboardSetReleases


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[GameCenterDetailRelationshipsLeaderboardSetReleasesDataInner]**](GameCenterDetailRelationshipsLeaderboardSetReleasesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_detail_relationships_leaderboard_set_releases import GameCenterDetailRelationshipsLeaderboardSetReleases

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailRelationshipsLeaderboardSetReleases from a JSON string
game_center_detail_relationships_leaderboard_set_releases_instance = GameCenterDetailRelationshipsLeaderboardSetReleases.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailRelationshipsLeaderboardSetReleases.to_json())

# convert the object into a dict
game_center_detail_relationships_leaderboard_set_releases_dict = game_center_detail_relationships_leaderboard_set_releases_instance.to_dict()
# create an instance of GameCenterDetailRelationshipsLeaderboardSetReleases from a dict
game_center_detail_relationships_leaderboard_set_releases_from_dict = GameCenterDetailRelationshipsLeaderboardSetReleases.from_dict(game_center_detail_relationships_leaderboard_set_releases_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


