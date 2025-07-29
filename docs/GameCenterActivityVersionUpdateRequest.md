# GameCenterActivityVersionUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterActivityVersionUpdateRequestData**](GameCenterActivityVersionUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.game_center_activity_version_update_request import GameCenterActivityVersionUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityVersionUpdateRequest from a JSON string
game_center_activity_version_update_request_instance = GameCenterActivityVersionUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityVersionUpdateRequest.to_json())

# convert the object into a dict
game_center_activity_version_update_request_dict = game_center_activity_version_update_request_instance.to_dict()
# create an instance of GameCenterActivityVersionUpdateRequest from a dict
game_center_activity_version_update_request_from_dict = GameCenterActivityVersionUpdateRequest.from_dict(game_center_activity_version_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


