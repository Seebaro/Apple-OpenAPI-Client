# GameCenterLeaderboardSetMemberLocalization


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterLeaderboardSetMemberLocalizationAttributes**](GameCenterLeaderboardSetMemberLocalizationAttributes.md) |  | [optional] 
**relationships** | [**GameCenterLeaderboardSetMemberLocalizationRelationships**](GameCenterLeaderboardSetMemberLocalizationRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_member_localization import GameCenterLeaderboardSetMemberLocalization

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetMemberLocalization from a JSON string
game_center_leaderboard_set_member_localization_instance = GameCenterLeaderboardSetMemberLocalization.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetMemberLocalization.to_json())

# convert the object into a dict
game_center_leaderboard_set_member_localization_dict = game_center_leaderboard_set_member_localization_instance.to_dict()
# create an instance of GameCenterLeaderboardSetMemberLocalization from a dict
game_center_leaderboard_set_member_localization_from_dict = GameCenterLeaderboardSetMemberLocalization.from_dict(game_center_leaderboard_set_member_localization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


