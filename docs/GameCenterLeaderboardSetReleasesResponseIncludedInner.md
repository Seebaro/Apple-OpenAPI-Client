# GameCenterLeaderboardSetReleasesResponseIncludedInner


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
from openapi_client.models.game_center_leaderboard_set_releases_response_included_inner import GameCenterLeaderboardSetReleasesResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetReleasesResponseIncludedInner from a JSON string
game_center_leaderboard_set_releases_response_included_inner_instance = GameCenterLeaderboardSetReleasesResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetReleasesResponseIncludedInner.to_json())

# convert the object into a dict
game_center_leaderboard_set_releases_response_included_inner_dict = game_center_leaderboard_set_releases_response_included_inner_instance.to_dict()
# create an instance of GameCenterLeaderboardSetReleasesResponseIncludedInner from a dict
game_center_leaderboard_set_releases_response_included_inner_from_dict = GameCenterLeaderboardSetReleasesResponseIncludedInner.from_dict(game_center_leaderboard_set_releases_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


