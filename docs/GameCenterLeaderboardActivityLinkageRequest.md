# GameCenterLeaderboardActivityLinkageRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterAchievementRelationshipsActivityData**](GameCenterAchievementRelationshipsActivityData.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_activity_linkage_request import GameCenterLeaderboardActivityLinkageRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardActivityLinkageRequest from a JSON string
game_center_leaderboard_activity_linkage_request_instance = GameCenterLeaderboardActivityLinkageRequest.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardActivityLinkageRequest.to_json())

# convert the object into a dict
game_center_leaderboard_activity_linkage_request_dict = game_center_leaderboard_activity_linkage_request_instance.to_dict()
# create an instance of GameCenterLeaderboardActivityLinkageRequest from a dict
game_center_leaderboard_activity_linkage_request_from_dict = GameCenterLeaderboardActivityLinkageRequest.from_dict(game_center_leaderboard_activity_linkage_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


