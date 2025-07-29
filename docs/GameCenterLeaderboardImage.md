# GameCenterLeaderboardImage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterAchievementImageAttributes**](GameCenterAchievementImageAttributes.md) |  | [optional] 
**relationships** | [**GameCenterLeaderboardImageRelationships**](GameCenterLeaderboardImageRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_image import GameCenterLeaderboardImage

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardImage from a JSON string
game_center_leaderboard_image_instance = GameCenterLeaderboardImage.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardImage.to_json())

# convert the object into a dict
game_center_leaderboard_image_dict = game_center_leaderboard_image_instance.to_dict()
# create an instance of GameCenterLeaderboardImage from a dict
game_center_leaderboard_image_from_dict = GameCenterLeaderboardImage.from_dict(game_center_leaderboard_image_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


