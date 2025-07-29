# GameCenterActivity


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
from openapi_client.models.game_center_activity import GameCenterActivity

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivity from a JSON string
game_center_activity_instance = GameCenterActivity.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivity.to_json())

# convert the object into a dict
game_center_activity_dict = game_center_activity_instance.to_dict()
# create an instance of GameCenterActivity from a dict
game_center_activity_from_dict = GameCenterActivity.from_dict(game_center_activity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


