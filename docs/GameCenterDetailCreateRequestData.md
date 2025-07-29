# GameCenterDetailCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterDetailCreateRequestDataAttributes**](GameCenterDetailCreateRequestDataAttributes.md) |  | [optional] 
**relationships** | [**AccessibilityDeclarationCreateRequestDataRelationships**](AccessibilityDeclarationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.game_center_detail_create_request_data import GameCenterDetailCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailCreateRequestData from a JSON string
game_center_detail_create_request_data_instance = GameCenterDetailCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailCreateRequestData.to_json())

# convert the object into a dict
game_center_detail_create_request_data_dict = game_center_detail_create_request_data_instance.to_dict()
# create an instance of GameCenterDetailCreateRequestData from a dict
game_center_detail_create_request_data_from_dict = GameCenterDetailCreateRequestData.from_dict(game_center_detail_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


