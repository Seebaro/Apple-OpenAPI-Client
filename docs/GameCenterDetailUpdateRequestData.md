# GameCenterDetailUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterDetailCreateRequestDataAttributes**](GameCenterDetailCreateRequestDataAttributes.md) |  | [optional] 
**relationships** | [**GameCenterDetailUpdateRequestDataRelationships**](GameCenterDetailUpdateRequestDataRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_detail_update_request_data import GameCenterDetailUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailUpdateRequestData from a JSON string
game_center_detail_update_request_data_instance = GameCenterDetailUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailUpdateRequestData.to_json())

# convert the object into a dict
game_center_detail_update_request_data_dict = game_center_detail_update_request_data_instance.to_dict()
# create an instance of GameCenterDetailUpdateRequestData from a dict
game_center_detail_update_request_data_from_dict = GameCenterDetailUpdateRequestData.from_dict(game_center_detail_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


