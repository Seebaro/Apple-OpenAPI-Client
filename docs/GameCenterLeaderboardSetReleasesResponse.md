# GameCenterLeaderboardSetReleasesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterLeaderboardSetRelease]**](GameCenterLeaderboardSetRelease.md) |  | 
**included** | [**List[GameCenterLeaderboardSetReleasesResponseIncludedInner]**](GameCenterLeaderboardSetReleasesResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_releases_response import GameCenterLeaderboardSetReleasesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetReleasesResponse from a JSON string
game_center_leaderboard_set_releases_response_instance = GameCenterLeaderboardSetReleasesResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetReleasesResponse.to_json())

# convert the object into a dict
game_center_leaderboard_set_releases_response_dict = game_center_leaderboard_set_releases_response_instance.to_dict()
# create an instance of GameCenterLeaderboardSetReleasesResponse from a dict
game_center_leaderboard_set_releases_response_from_dict = GameCenterLeaderboardSetReleasesResponse.from_dict(game_center_leaderboard_set_releases_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


