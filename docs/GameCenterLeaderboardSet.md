# GameCenterLeaderboardSet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterLeaderboardSetAttributes**](GameCenterLeaderboardSetAttributes.md) |  | [optional] 
**relationships** | [**GameCenterLeaderboardSetRelationships**](GameCenterLeaderboardSetRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_set import GameCenterLeaderboardSet

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSet from a JSON string
game_center_leaderboard_set_instance = GameCenterLeaderboardSet.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSet.to_json())

# convert the object into a dict
game_center_leaderboard_set_dict = game_center_leaderboard_set_instance.to_dict()
# create an instance of GameCenterLeaderboardSet from a dict
game_center_leaderboard_set_from_dict = GameCenterLeaderboardSet.from_dict(game_center_leaderboard_set_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


