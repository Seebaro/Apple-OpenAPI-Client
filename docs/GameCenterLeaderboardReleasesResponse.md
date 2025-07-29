# GameCenterLeaderboardReleasesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterLeaderboardRelease]**](GameCenterLeaderboardRelease.md) |  | 
**included** | [**List[GameCenterLeaderboardReleasesResponseIncludedInner]**](GameCenterLeaderboardReleasesResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_releases_response import GameCenterLeaderboardReleasesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardReleasesResponse from a JSON string
game_center_leaderboard_releases_response_instance = GameCenterLeaderboardReleasesResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardReleasesResponse.to_json())

# convert the object into a dict
game_center_leaderboard_releases_response_dict = game_center_leaderboard_releases_response_instance.to_dict()
# create an instance of GameCenterLeaderboardReleasesResponse from a dict
game_center_leaderboard_releases_response_from_dict = GameCenterLeaderboardReleasesResponse.from_dict(game_center_leaderboard_releases_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


