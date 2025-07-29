# GameCenterLeaderboardSetImageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterLeaderboardSetImage**](GameCenterLeaderboardSetImage.md) |  | 
**included** | [**List[GameCenterLeaderboardSetLocalization]**](GameCenterLeaderboardSetLocalization.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_image_response import GameCenterLeaderboardSetImageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetImageResponse from a JSON string
game_center_leaderboard_set_image_response_instance = GameCenterLeaderboardSetImageResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetImageResponse.to_json())

# convert the object into a dict
game_center_leaderboard_set_image_response_dict = game_center_leaderboard_set_image_response_instance.to_dict()
# create an instance of GameCenterLeaderboardSetImageResponse from a dict
game_center_leaderboard_set_image_response_from_dict = GameCenterLeaderboardSetImageResponse.from_dict(game_center_leaderboard_set_image_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


