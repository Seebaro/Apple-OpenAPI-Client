# GameCenterLeaderboard


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterLeaderboardAttributes**](GameCenterLeaderboardAttributes.md) |  | [optional] 
**relationships** | [**GameCenterLeaderboardRelationships**](GameCenterLeaderboardRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard import GameCenterLeaderboard

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboard from a JSON string
game_center_leaderboard_instance = GameCenterLeaderboard.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboard.to_json())

# convert the object into a dict
game_center_leaderboard_dict = game_center_leaderboard_instance.to_dict()
# create an instance of GameCenterLeaderboard from a dict
game_center_leaderboard_from_dict = GameCenterLeaderboard.from_dict(game_center_leaderboard_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


