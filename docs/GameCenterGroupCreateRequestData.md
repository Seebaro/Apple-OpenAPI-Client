# GameCenterGroupCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterGroupAttributes**](GameCenterGroupAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_group_create_request_data import GameCenterGroupCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterGroupCreateRequestData from a JSON string
game_center_group_create_request_data_instance = GameCenterGroupCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterGroupCreateRequestData.to_json())

# convert the object into a dict
game_center_group_create_request_data_dict = game_center_group_create_request_data_instance.to_dict()
# create an instance of GameCenterGroupCreateRequestData from a dict
game_center_group_create_request_data_from_dict = GameCenterGroupCreateRequestData.from_dict(game_center_group_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


