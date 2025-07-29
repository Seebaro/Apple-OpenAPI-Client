# GameCenterAchievementReleasesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterAchievementRelationshipsReleasesDataInner]**](GameCenterAchievementRelationshipsReleasesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievement_releases_linkages_response import GameCenterAchievementReleasesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementReleasesLinkagesResponse from a JSON string
game_center_achievement_releases_linkages_response_instance = GameCenterAchievementReleasesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementReleasesLinkagesResponse.to_json())

# convert the object into a dict
game_center_achievement_releases_linkages_response_dict = game_center_achievement_releases_linkages_response_instance.to_dict()
# create an instance of GameCenterAchievementReleasesLinkagesResponse from a dict
game_center_achievement_releases_linkages_response_from_dict = GameCenterAchievementReleasesLinkagesResponse.from_dict(game_center_achievement_releases_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


