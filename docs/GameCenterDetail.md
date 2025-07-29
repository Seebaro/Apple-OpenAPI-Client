# GameCenterDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterDetailAttributes**](GameCenterDetailAttributes.md) |  | [optional] 
**relationships** | [**GameCenterDetailRelationships**](GameCenterDetailRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_detail import GameCenterDetail

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetail from a JSON string
game_center_detail_instance = GameCenterDetail.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetail.to_json())

# convert the object into a dict
game_center_detail_dict = game_center_detail_instance.to_dict()
# create an instance of GameCenterDetail from a dict
game_center_detail_from_dict = GameCenterDetail.from_dict(game_center_detail_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


