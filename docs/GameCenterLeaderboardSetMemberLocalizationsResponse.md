# GameCenterLeaderboardSetMemberLocalizationsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterLeaderboardSetMemberLocalization]**](GameCenterLeaderboardSetMemberLocalization.md) |  | 
**included** | [**List[GameCenterLeaderboardSetMemberLocalizationsResponseIncludedInner]**](GameCenterLeaderboardSetMemberLocalizationsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_member_localizations_response import GameCenterLeaderboardSetMemberLocalizationsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetMemberLocalizationsResponse from a JSON string
game_center_leaderboard_set_member_localizations_response_instance = GameCenterLeaderboardSetMemberLocalizationsResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetMemberLocalizationsResponse.to_json())

# convert the object into a dict
game_center_leaderboard_set_member_localizations_response_dict = game_center_leaderboard_set_member_localizations_response_instance.to_dict()
# create an instance of GameCenterLeaderboardSetMemberLocalizationsResponse from a dict
game_center_leaderboard_set_member_localizations_response_from_dict = GameCenterLeaderboardSetMemberLocalizationsResponse.from_dict(game_center_leaderboard_set_member_localizations_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


