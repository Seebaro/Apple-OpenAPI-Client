# GameCenterActivityImageCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterActivityImageCreateRequestData**](GameCenterActivityImageCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.game_center_activity_image_create_request import GameCenterActivityImageCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityImageCreateRequest from a JSON string
game_center_activity_image_create_request_instance = GameCenterActivityImageCreateRequest.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityImageCreateRequest.to_json())

# convert the object into a dict
game_center_activity_image_create_request_dict = game_center_activity_image_create_request_instance.to_dict()
# create an instance of GameCenterActivityImageCreateRequest from a dict
game_center_activity_image_create_request_from_dict = GameCenterActivityImageCreateRequest.from_dict(game_center_activity_image_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


