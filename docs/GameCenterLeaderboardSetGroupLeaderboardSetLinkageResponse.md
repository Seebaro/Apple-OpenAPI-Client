# GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterDetailRelationshipsGameCenterLeaderboardSetsDataInner**](GameCenterDetailRelationshipsGameCenterLeaderboardSetsDataInner.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_group_leaderboard_set_linkage_response import GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse from a JSON string
game_center_leaderboard_set_group_leaderboard_set_linkage_response_instance = GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse.to_json())

# convert the object into a dict
game_center_leaderboard_set_group_leaderboard_set_linkage_response_dict = game_center_leaderboard_set_group_leaderboard_set_linkage_response_instance.to_dict()
# create an instance of GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse from a dict
game_center_leaderboard_set_group_leaderboard_set_linkage_response_from_dict = GameCenterLeaderboardSetGroupLeaderboardSetLinkageResponse.from_dict(game_center_leaderboard_set_group_leaderboard_set_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


