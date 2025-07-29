# GameCenterAppVersion


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterAppVersionAttributes**](GameCenterAppVersionAttributes.md) |  | [optional] 
**relationships** | [**GameCenterAppVersionRelationships**](GameCenterAppVersionRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_app_version import GameCenterAppVersion

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAppVersion from a JSON string
game_center_app_version_instance = GameCenterAppVersion.from_json(json)
# print the JSON string representation of the object
print(GameCenterAppVersion.to_json())

# convert the object into a dict
game_center_app_version_dict = game_center_app_version_instance.to_dict()
# create an instance of GameCenterAppVersion from a dict
game_center_app_version_from_dict = GameCenterAppVersion.from_dict(game_center_app_version_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


