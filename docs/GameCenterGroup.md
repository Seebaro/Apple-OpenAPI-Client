# GameCenterGroup


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterGroupAttributes**](GameCenterGroupAttributes.md) |  | [optional] 
**relationships** | [**GameCenterGroupRelationships**](GameCenterGroupRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_group import GameCenterGroup

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterGroup from a JSON string
game_center_group_instance = GameCenterGroup.from_json(json)
# print the JSON string representation of the object
print(GameCenterGroup.to_json())

# convert the object into a dict
game_center_group_dict = game_center_group_instance.to_dict()
# create an instance of GameCenterGroup from a dict
game_center_group_from_dict = GameCenterGroup.from_dict(game_center_group_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


