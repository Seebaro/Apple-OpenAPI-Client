# GameCenterLeaderboardSetsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterLeaderboardSet]**](GameCenterLeaderboardSet.md) |  | 
**included** | [**List[GameCenterLeaderboardSetsResponseIncludedInner]**](GameCenterLeaderboardSetsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_sets_response import GameCenterLeaderboardSetsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetsResponse from a JSON string
game_center_leaderboard_sets_response_instance = GameCenterLeaderboardSetsResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetsResponse.to_json())

# convert the object into a dict
game_center_leaderboard_sets_response_dict = game_center_leaderboard_sets_response_instance.to_dict()
# create an instance of GameCenterLeaderboardSetsResponse from a dict
game_center_leaderboard_sets_response_from_dict = GameCenterLeaderboardSetsResponse.from_dict(game_center_leaderboard_sets_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


