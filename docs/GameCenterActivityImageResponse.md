# GameCenterActivityImageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterActivityImage**](GameCenterActivityImage.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_activity_image_response import GameCenterActivityImageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityImageResponse from a JSON string
game_center_activity_image_response_instance = GameCenterActivityImageResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityImageResponse.to_json())

# convert the object into a dict
game_center_activity_image_response_dict = game_center_activity_image_response_instance.to_dict()
# create an instance of GameCenterActivityImageResponse from a dict
game_center_activity_image_response_from_dict = GameCenterActivityImageResponse.from_dict(game_center_activity_image_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


