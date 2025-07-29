# GameCenterDetailCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterDetailCreateRequestData**](GameCenterDetailCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.game_center_detail_create_request import GameCenterDetailCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailCreateRequest from a JSON string
game_center_detail_create_request_instance = GameCenterDetailCreateRequest.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailCreateRequest.to_json())

# convert the object into a dict
game_center_detail_create_request_dict = game_center_detail_create_request_instance.to_dict()
# create an instance of GameCenterDetailCreateRequest from a dict
game_center_detail_create_request_from_dict = GameCenterDetailCreateRequest.from_dict(game_center_detail_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


