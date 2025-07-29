# GameCenterLeaderboardResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterLeaderboard**](GameCenterLeaderboard.md) |  | 
**included** | [**List[GameCenterLeaderboardsResponseIncludedInner]**](GameCenterLeaderboardsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_response import GameCenterLeaderboardResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardResponse from a JSON string
game_center_leaderboard_response_instance = GameCenterLeaderboardResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardResponse.to_json())

# convert the object into a dict
game_center_leaderboard_response_dict = game_center_leaderboard_response_instance.to_dict()
# create an instance of GameCenterLeaderboardResponse from a dict
game_center_leaderboard_response_from_dict = GameCenterLeaderboardResponse.from_dict(game_center_leaderboard_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


