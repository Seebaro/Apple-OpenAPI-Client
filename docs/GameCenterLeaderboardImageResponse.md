# GameCenterLeaderboardImageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterLeaderboardImage**](GameCenterLeaderboardImage.md) |  | 
**included** | [**List[GameCenterLeaderboardLocalization]**](GameCenterLeaderboardLocalization.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_image_response import GameCenterLeaderboardImageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardImageResponse from a JSON string
game_center_leaderboard_image_response_instance = GameCenterLeaderboardImageResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardImageResponse.to_json())

# convert the object into a dict
game_center_leaderboard_image_response_dict = game_center_leaderboard_image_response_instance.to_dict()
# create an instance of GameCenterLeaderboardImageResponse from a dict
game_center_leaderboard_image_response_from_dict = GameCenterLeaderboardImageResponse.from_dict(game_center_leaderboard_image_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


