# GameCenterActivityUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterActivityUpdateRequestData**](GameCenterActivityUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.game_center_activity_update_request import GameCenterActivityUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityUpdateRequest from a JSON string
game_center_activity_update_request_instance = GameCenterActivityUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityUpdateRequest.to_json())

# convert the object into a dict
game_center_activity_update_request_dict = game_center_activity_update_request_instance.to_dict()
# create an instance of GameCenterActivityUpdateRequest from a dict
game_center_activity_update_request_from_dict = GameCenterActivityUpdateRequest.from_dict(game_center_activity_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


