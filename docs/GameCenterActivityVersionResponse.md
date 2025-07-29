# GameCenterActivityVersionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterActivityVersion**](GameCenterActivityVersion.md) |  | 
**included** | [**List[GameCenterActivityVersionsResponseIncludedInner]**](GameCenterActivityVersionsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_activity_version_response import GameCenterActivityVersionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityVersionResponse from a JSON string
game_center_activity_version_response_instance = GameCenterActivityVersionResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityVersionResponse.to_json())

# convert the object into a dict
game_center_activity_version_response_dict = game_center_activity_version_response_instance.to_dict()
# create an instance of GameCenterActivityVersionResponse from a dict
game_center_activity_version_response_from_dict = GameCenterActivityVersionResponse.from_dict(game_center_activity_version_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


