# GameCenterLeaderboardSetReleaseCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**game_center_detail** | [**GameCenterAchievementReleaseCreateRequestDataRelationshipsGameCenterDetail**](GameCenterAchievementReleaseCreateRequestDataRelationshipsGameCenterDetail.md) |  | 
**game_center_leaderboard_set** | [**GameCenterLeaderboardSetLocalizationCreateRequestDataRelationshipsGameCenterLeaderboardSet**](GameCenterLeaderboardSetLocalizationCreateRequestDataRelationshipsGameCenterLeaderboardSet.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_release_create_request_data_relationships import GameCenterLeaderboardSetReleaseCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetReleaseCreateRequestDataRelationships from a JSON string
game_center_leaderboard_set_release_create_request_data_relationships_instance = GameCenterLeaderboardSetReleaseCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetReleaseCreateRequestDataRelationships.to_json())

# convert the object into a dict
game_center_leaderboard_set_release_create_request_data_relationships_dict = game_center_leaderboard_set_release_create_request_data_relationships_instance.to_dict()
# create an instance of GameCenterLeaderboardSetReleaseCreateRequestDataRelationships from a dict
game_center_leaderboard_set_release_create_request_data_relationships_from_dict = GameCenterLeaderboardSetReleaseCreateRequestDataRelationships.from_dict(game_center_leaderboard_set_release_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


