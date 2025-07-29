# GameCenterActivityVersion


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterActivityVersionAttributes**](GameCenterActivityVersionAttributes.md) |  | [optional] 
**relationships** | [**GameCenterActivityVersionRelationships**](GameCenterActivityVersionRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_activity_version import GameCenterActivityVersion

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityVersion from a JSON string
game_center_activity_version_instance = GameCenterActivityVersion.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityVersion.to_json())

# convert the object into a dict
game_center_activity_version_dict = game_center_activity_version_instance.to_dict()
# create an instance of GameCenterActivityVersion from a dict
game_center_activity_version_from_dict = GameCenterActivityVersion.from_dict(game_center_activity_version_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


