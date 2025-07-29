# GameCenterLeaderboardSetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterLeaderboardSet**](GameCenterLeaderboardSet.md) |  | 
**included** | [**List[GameCenterLeaderboardSetsResponseIncludedInner]**](GameCenterLeaderboardSetsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_response import GameCenterLeaderboardSetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetResponse from a JSON string
game_center_leaderboard_set_response_instance = GameCenterLeaderboardSetResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetResponse.to_json())

# convert the object into a dict
game_center_leaderboard_set_response_dict = game_center_leaderboard_set_response_instance.to_dict()
# create an instance of GameCenterLeaderboardSetResponse from a dict
game_center_leaderboard_set_response_from_dict = GameCenterLeaderboardSetResponse.from_dict(game_center_leaderboard_set_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


