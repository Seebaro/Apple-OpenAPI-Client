# GameCenterLeaderboardReleasesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterDetailRelationshipsLeaderboardReleasesDataInner]**](GameCenterDetailRelationshipsLeaderboardReleasesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_releases_linkages_response import GameCenterLeaderboardReleasesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardReleasesLinkagesResponse from a JSON string
game_center_leaderboard_releases_linkages_response_instance = GameCenterLeaderboardReleasesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardReleasesLinkagesResponse.to_json())

# convert the object into a dict
game_center_leaderboard_releases_linkages_response_dict = game_center_leaderboard_releases_linkages_response_instance.to_dict()
# create an instance of GameCenterLeaderboardReleasesLinkagesResponse from a dict
game_center_leaderboard_releases_linkages_response_from_dict = GameCenterLeaderboardReleasesLinkagesResponse.from_dict(game_center_leaderboard_releases_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


