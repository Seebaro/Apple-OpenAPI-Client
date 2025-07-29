# GameCenterLeaderboardSetUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterLeaderboardSetUpdateRequestData**](GameCenterLeaderboardSetUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_update_request import GameCenterLeaderboardSetUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetUpdateRequest from a JSON string
game_center_leaderboard_set_update_request_instance = GameCenterLeaderboardSetUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetUpdateRequest.to_json())

# convert the object into a dict
game_center_leaderboard_set_update_request_dict = game_center_leaderboard_set_update_request_instance.to_dict()
# create an instance of GameCenterLeaderboardSetUpdateRequest from a dict
game_center_leaderboard_set_update_request_from_dict = GameCenterLeaderboardSetUpdateRequest.from_dict(game_center_leaderboard_set_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


