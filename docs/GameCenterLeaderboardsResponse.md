# GameCenterLeaderboardsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterLeaderboard]**](GameCenterLeaderboard.md) |  | 
**included** | [**List[GameCenterLeaderboardsResponseIncludedInner]**](GameCenterLeaderboardsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboards_response import GameCenterLeaderboardsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardsResponse from a JSON string
game_center_leaderboards_response_instance = GameCenterLeaderboardsResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardsResponse.to_json())

# convert the object into a dict
game_center_leaderboards_response_dict = game_center_leaderboards_response_instance.to_dict()
# create an instance of GameCenterLeaderboardsResponse from a dict
game_center_leaderboards_response_from_dict = GameCenterLeaderboardsResponse.from_dict(game_center_leaderboards_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


