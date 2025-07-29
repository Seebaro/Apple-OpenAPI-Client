# GameCenterDetailUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterDetailUpdateRequestData**](GameCenterDetailUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.game_center_detail_update_request import GameCenterDetailUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailUpdateRequest from a JSON string
game_center_detail_update_request_instance = GameCenterDetailUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailUpdateRequest.to_json())

# convert the object into a dict
game_center_detail_update_request_dict = game_center_detail_update_request_instance.to_dict()
# create an instance of GameCenterDetailUpdateRequest from a dict
game_center_detail_update_request_from_dict = GameCenterDetailUpdateRequest.from_dict(game_center_detail_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


