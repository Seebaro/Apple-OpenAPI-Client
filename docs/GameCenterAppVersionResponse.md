# GameCenterAppVersionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterAppVersion**](GameCenterAppVersion.md) |  | 
**included** | [**List[GameCenterAppVersionsResponseIncludedInner]**](GameCenterAppVersionsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_app_version_response import GameCenterAppVersionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAppVersionResponse from a JSON string
game_center_app_version_response_instance = GameCenterAppVersionResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterAppVersionResponse.to_json())

# convert the object into a dict
game_center_app_version_response_dict = game_center_app_version_response_instance.to_dict()
# create an instance of GameCenterAppVersionResponse from a dict
game_center_app_version_response_from_dict = GameCenterAppVersionResponse.from_dict(game_center_app_version_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


