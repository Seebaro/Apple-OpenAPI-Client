# GameCenterAchievementsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterActivityAttributes**](GameCenterActivityAttributes.md) |  | [optional] 
**relationships** | [**GameCenterActivityRelationships**](GameCenterActivityRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievements_response_included_inner import GameCenterAchievementsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementsResponseIncludedInner from a JSON string
game_center_achievements_response_included_inner_instance = GameCenterAchievementsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementsResponseIncludedInner.to_json())

# convert the object into a dict
game_center_achievements_response_included_inner_dict = game_center_achievements_response_included_inner_instance.to_dict()
# create an instance of GameCenterAchievementsResponseIncludedInner from a dict
game_center_achievements_response_included_inner_from_dict = GameCenterAchievementsResponseIncludedInner.from_dict(game_center_achievements_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


