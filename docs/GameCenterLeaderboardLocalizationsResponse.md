# GameCenterLeaderboardLocalizationsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterLeaderboardLocalization]**](GameCenterLeaderboardLocalization.md) |  | 
**included** | [**List[GameCenterLeaderboardLocalizationsResponseIncludedInner]**](GameCenterLeaderboardLocalizationsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_localizations_response import GameCenterLeaderboardLocalizationsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardLocalizationsResponse from a JSON string
game_center_leaderboard_localizations_response_instance = GameCenterLeaderboardLocalizationsResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardLocalizationsResponse.to_json())

# convert the object into a dict
game_center_leaderboard_localizations_response_dict = game_center_leaderboard_localizations_response_instance.to_dict()
# create an instance of GameCenterLeaderboardLocalizationsResponse from a dict
game_center_leaderboard_localizations_response_from_dict = GameCenterLeaderboardLocalizationsResponse.from_dict(game_center_leaderboard_localizations_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


