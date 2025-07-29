# GameCenterDetailGameCenterAchievementsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterAchievementLocalizationRelationshipsGameCenterAchievementData]**](GameCenterAchievementLocalizationRelationshipsGameCenterAchievementData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_detail_game_center_achievements_linkages_response import GameCenterDetailGameCenterAchievementsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailGameCenterAchievementsLinkagesResponse from a JSON string
game_center_detail_game_center_achievements_linkages_response_instance = GameCenterDetailGameCenterAchievementsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailGameCenterAchievementsLinkagesResponse.to_json())

# convert the object into a dict
game_center_detail_game_center_achievements_linkages_response_dict = game_center_detail_game_center_achievements_linkages_response_instance.to_dict()
# create an instance of GameCenterDetailGameCenterAchievementsLinkagesResponse from a dict
game_center_detail_game_center_achievements_linkages_response_from_dict = GameCenterDetailGameCenterAchievementsLinkagesResponse.from_dict(game_center_detail_game_center_achievements_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


