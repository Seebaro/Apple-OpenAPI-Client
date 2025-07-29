# GameCenterLeaderboardSetMemberLocalizationCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterLeaderboardSetMemberLocalizationAttributes**](GameCenterLeaderboardSetMemberLocalizationAttributes.md) |  | [optional] 
**relationships** | [**GameCenterLeaderboardSetMemberLocalizationCreateRequestDataRelationships**](GameCenterLeaderboardSetMemberLocalizationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_member_localization_create_request_data import GameCenterLeaderboardSetMemberLocalizationCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetMemberLocalizationCreateRequestData from a JSON string
game_center_leaderboard_set_member_localization_create_request_data_instance = GameCenterLeaderboardSetMemberLocalizationCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetMemberLocalizationCreateRequestData.to_json())

# convert the object into a dict
game_center_leaderboard_set_member_localization_create_request_data_dict = game_center_leaderboard_set_member_localization_create_request_data_instance.to_dict()
# create an instance of GameCenterLeaderboardSetMemberLocalizationCreateRequestData from a dict
game_center_leaderboard_set_member_localization_create_request_data_from_dict = GameCenterLeaderboardSetMemberLocalizationCreateRequestData.from_dict(game_center_leaderboard_set_member_localization_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


