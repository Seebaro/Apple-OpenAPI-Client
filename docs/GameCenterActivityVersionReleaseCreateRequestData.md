# GameCenterActivityVersionReleaseCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**GameCenterActivityVersionReleaseCreateRequestDataRelationships**](GameCenterActivityVersionReleaseCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.game_center_activity_version_release_create_request_data import GameCenterActivityVersionReleaseCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityVersionReleaseCreateRequestData from a JSON string
game_center_activity_version_release_create_request_data_instance = GameCenterActivityVersionReleaseCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityVersionReleaseCreateRequestData.to_json())

# convert the object into a dict
game_center_activity_version_release_create_request_data_dict = game_center_activity_version_release_create_request_data_instance.to_dict()
# create an instance of GameCenterActivityVersionReleaseCreateRequestData from a dict
game_center_activity_version_release_create_request_data_from_dict = GameCenterActivityVersionReleaseCreateRequestData.from_dict(game_center_activity_version_release_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


