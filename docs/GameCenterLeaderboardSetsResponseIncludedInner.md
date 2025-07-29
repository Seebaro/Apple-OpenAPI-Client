# GameCenterLeaderboardSetsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterAchievementReleaseAttributes**](GameCenterAchievementReleaseAttributes.md) |  | [optional] 
**relationships** | [**GameCenterLeaderboardSetReleaseRelationships**](GameCenterLeaderboardSetReleaseRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_sets_response_included_inner import GameCenterLeaderboardSetsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetsResponseIncludedInner from a JSON string
game_center_leaderboard_sets_response_included_inner_instance = GameCenterLeaderboardSetsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetsResponseIncludedInner.to_json())

# convert the object into a dict
game_center_leaderboard_sets_response_included_inner_dict = game_center_leaderboard_sets_response_included_inner_instance.to_dict()
# create an instance of GameCenterLeaderboardSetsResponseIncludedInner from a dict
game_center_leaderboard_sets_response_included_inner_from_dict = GameCenterLeaderboardSetsResponseIncludedInner.from_dict(game_center_leaderboard_sets_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


