# GameCenterAchievementReleasesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterAchievementRelease]**](GameCenterAchievementRelease.md) |  | 
**included** | [**List[GameCenterAchievementReleasesResponseIncludedInner]**](GameCenterAchievementReleasesResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievement_releases_response import GameCenterAchievementReleasesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementReleasesResponse from a JSON string
game_center_achievement_releases_response_instance = GameCenterAchievementReleasesResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementReleasesResponse.to_json())

# convert the object into a dict
game_center_achievement_releases_response_dict = game_center_achievement_releases_response_instance.to_dict()
# create an instance of GameCenterAchievementReleasesResponse from a dict
game_center_achievement_releases_response_from_dict = GameCenterAchievementReleasesResponse.from_dict(game_center_achievement_releases_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


