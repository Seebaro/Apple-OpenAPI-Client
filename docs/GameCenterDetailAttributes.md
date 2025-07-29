# GameCenterDetailAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**arcade_enabled** | **bool** |  | [optional] 
**challenge_enabled** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_detail_attributes import GameCenterDetailAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailAttributes from a JSON string
game_center_detail_attributes_instance = GameCenterDetailAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailAttributes.to_json())

# convert the object into a dict
game_center_detail_attributes_dict = game_center_detail_attributes_instance.to_dict()
# create an instance of GameCenterDetailAttributes from a dict
game_center_detail_attributes_from_dict = GameCenterDetailAttributes.from_dict(game_center_detail_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


