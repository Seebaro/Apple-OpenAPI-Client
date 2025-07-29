# GameCenterLeaderboardSetLocalizationsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterLeaderboardSetImageRelationshipsGameCenterLeaderboardSetLocalizationData]**](GameCenterLeaderboardSetImageRelationshipsGameCenterLeaderboardSetLocalizationData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_localizations_linkages_response import GameCenterLeaderboardSetLocalizationsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetLocalizationsLinkagesResponse from a JSON string
game_center_leaderboard_set_localizations_linkages_response_instance = GameCenterLeaderboardSetLocalizationsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetLocalizationsLinkagesResponse.to_json())

# convert the object into a dict
game_center_leaderboard_set_localizations_linkages_response_dict = game_center_leaderboard_set_localizations_linkages_response_instance.to_dict()
# create an instance of GameCenterLeaderboardSetLocalizationsLinkagesResponse from a dict
game_center_leaderboard_set_localizations_linkages_response_from_dict = GameCenterLeaderboardSetLocalizationsLinkagesResponse.from_dict(game_center_leaderboard_set_localizations_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


