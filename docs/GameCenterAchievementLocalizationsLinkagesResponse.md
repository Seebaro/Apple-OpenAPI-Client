# GameCenterAchievementLocalizationsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterAchievementImageRelationshipsGameCenterAchievementLocalizationData]**](GameCenterAchievementImageRelationshipsGameCenterAchievementLocalizationData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievement_localizations_linkages_response import GameCenterAchievementLocalizationsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementLocalizationsLinkagesResponse from a JSON string
game_center_achievement_localizations_linkages_response_instance = GameCenterAchievementLocalizationsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementLocalizationsLinkagesResponse.to_json())

# convert the object into a dict
game_center_achievement_localizations_linkages_response_dict = game_center_achievement_localizations_linkages_response_instance.to_dict()
# create an instance of GameCenterAchievementLocalizationsLinkagesResponse from a dict
game_center_achievement_localizations_linkages_response_from_dict = GameCenterAchievementLocalizationsLinkagesResponse.from_dict(game_center_achievement_localizations_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


