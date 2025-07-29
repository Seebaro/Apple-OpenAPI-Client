# GameCenterActivityVersionRelease


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**relationships** | [**GameCenterActivityVersionReleaseRelationships**](GameCenterActivityVersionReleaseRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_activity_version_release import GameCenterActivityVersionRelease

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityVersionRelease from a JSON string
game_center_activity_version_release_instance = GameCenterActivityVersionRelease.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityVersionRelease.to_json())

# convert the object into a dict
game_center_activity_version_release_dict = game_center_activity_version_release_instance.to_dict()
# create an instance of GameCenterActivityVersionRelease from a dict
game_center_activity_version_release_from_dict = GameCenterActivityVersionRelease.from_dict(game_center_activity_version_release_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


