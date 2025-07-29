# GameCenterAchievementsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterAchievement]**](GameCenterAchievement.md) |  | 
**included** | [**List[GameCenterAchievementsResponseIncludedInner]**](GameCenterAchievementsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievements_response import GameCenterAchievementsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementsResponse from a JSON string
game_center_achievements_response_instance = GameCenterAchievementsResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementsResponse.to_json())

# convert the object into a dict
game_center_achievements_response_dict = game_center_achievements_response_instance.to_dict()
# create an instance of GameCenterAchievementsResponse from a dict
game_center_achievements_response_from_dict = GameCenterAchievementsResponse.from_dict(game_center_achievements_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


