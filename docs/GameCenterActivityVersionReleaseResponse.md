# GameCenterActivityVersionReleaseResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterActivityVersionRelease**](GameCenterActivityVersionRelease.md) |  | 
**included** | [**List[GameCenterActivityVersion]**](GameCenterActivityVersion.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_activity_version_release_response import GameCenterActivityVersionReleaseResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityVersionReleaseResponse from a JSON string
game_center_activity_version_release_response_instance = GameCenterActivityVersionReleaseResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityVersionReleaseResponse.to_json())

# convert the object into a dict
game_center_activity_version_release_response_dict = game_center_activity_version_release_response_instance.to_dict()
# create an instance of GameCenterActivityVersionReleaseResponse from a dict
game_center_activity_version_release_response_from_dict = GameCenterActivityVersionReleaseResponse.from_dict(game_center_activity_version_release_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


