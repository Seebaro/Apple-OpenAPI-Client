# GameCenterLeaderboardSetReleaseResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterLeaderboardSetRelease**](GameCenterLeaderboardSetRelease.md) |  | 
**included** | [**List[GameCenterLeaderboardSetReleasesResponseIncludedInner]**](GameCenterLeaderboardSetReleasesResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_release_response import GameCenterLeaderboardSetReleaseResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetReleaseResponse from a JSON string
game_center_leaderboard_set_release_response_instance = GameCenterLeaderboardSetReleaseResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetReleaseResponse.to_json())

# convert the object into a dict
game_center_leaderboard_set_release_response_dict = game_center_leaderboard_set_release_response_instance.to_dict()
# create an instance of GameCenterLeaderboardSetReleaseResponse from a dict
game_center_leaderboard_set_release_response_from_dict = GameCenterLeaderboardSetReleaseResponse.from_dict(game_center_leaderboard_set_release_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


