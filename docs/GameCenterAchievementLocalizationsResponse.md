# GameCenterAchievementLocalizationsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterAchievementLocalization]**](GameCenterAchievementLocalization.md) |  | 
**included** | [**List[GameCenterAchievementLocalizationsResponseIncludedInner]**](GameCenterAchievementLocalizationsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievement_localizations_response import GameCenterAchievementLocalizationsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementLocalizationsResponse from a JSON string
game_center_achievement_localizations_response_instance = GameCenterAchievementLocalizationsResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementLocalizationsResponse.to_json())

# convert the object into a dict
game_center_achievement_localizations_response_dict = game_center_achievement_localizations_response_instance.to_dict()
# create an instance of GameCenterAchievementLocalizationsResponse from a dict
game_center_achievement_localizations_response_from_dict = GameCenterAchievementLocalizationsResponse.from_dict(game_center_achievement_localizations_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


