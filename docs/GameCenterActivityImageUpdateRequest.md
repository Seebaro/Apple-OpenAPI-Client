# GameCenterActivityImageUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterActivityImageUpdateRequestData**](GameCenterActivityImageUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.game_center_activity_image_update_request import GameCenterActivityImageUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityImageUpdateRequest from a JSON string
game_center_activity_image_update_request_instance = GameCenterActivityImageUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityImageUpdateRequest.to_json())

# convert the object into a dict
game_center_activity_image_update_request_dict = game_center_activity_image_update_request_instance.to_dict()
# create an instance of GameCenterActivityImageUpdateRequest from a dict
game_center_activity_image_update_request_from_dict = GameCenterActivityImageUpdateRequest.from_dict(game_center_activity_image_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


