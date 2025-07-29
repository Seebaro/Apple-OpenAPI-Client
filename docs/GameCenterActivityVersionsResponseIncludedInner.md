# GameCenterActivityVersionsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterAchievementImageAttributes**](GameCenterAchievementImageAttributes.md) |  | [optional] 
**relationships** | [**GameCenterActivityVersionReleaseRelationships**](GameCenterActivityVersionReleaseRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_activity_versions_response_included_inner import GameCenterActivityVersionsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityVersionsResponseIncludedInner from a JSON string
game_center_activity_versions_response_included_inner_instance = GameCenterActivityVersionsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityVersionsResponseIncludedInner.to_json())

# convert the object into a dict
game_center_activity_versions_response_included_inner_dict = game_center_activity_versions_response_included_inner_instance.to_dict()
# create an instance of GameCenterActivityVersionsResponseIncludedInner from a dict
game_center_activity_versions_response_included_inner_from_dict = GameCenterActivityVersionsResponseIncludedInner.from_dict(game_center_activity_versions_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


