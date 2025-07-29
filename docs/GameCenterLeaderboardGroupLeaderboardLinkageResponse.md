# GameCenterLeaderboardGroupLeaderboardLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterActivityRelationshipsLeaderboardsDataInner**](GameCenterActivityRelationshipsLeaderboardsDataInner.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_group_leaderboard_linkage_response import GameCenterLeaderboardGroupLeaderboardLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardGroupLeaderboardLinkageResponse from a JSON string
game_center_leaderboard_group_leaderboard_linkage_response_instance = GameCenterLeaderboardGroupLeaderboardLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardGroupLeaderboardLinkageResponse.to_json())

# convert the object into a dict
game_center_leaderboard_group_leaderboard_linkage_response_dict = game_center_leaderboard_group_leaderboard_linkage_response_instance.to_dict()
# create an instance of GameCenterLeaderboardGroupLeaderboardLinkageResponse from a dict
game_center_leaderboard_group_leaderboard_linkage_response_from_dict = GameCenterLeaderboardGroupLeaderboardLinkageResponse.from_dict(game_center_leaderboard_group_leaderboard_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


