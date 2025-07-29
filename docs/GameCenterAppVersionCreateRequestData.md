# GameCenterAppVersionCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**AlternativeDistributionPackageCreateRequestDataRelationships**](AlternativeDistributionPackageCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.game_center_app_version_create_request_data import GameCenterAppVersionCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAppVersionCreateRequestData from a JSON string
game_center_app_version_create_request_data_instance = GameCenterAppVersionCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterAppVersionCreateRequestData.to_json())

# convert the object into a dict
game_center_app_version_create_request_data_dict = game_center_app_version_create_request_data_instance.to_dict()
# create an instance of GameCenterAppVersionCreateRequestData from a dict
game_center_app_version_create_request_data_from_dict = GameCenterAppVersionCreateRequestData.from_dict(game_center_app_version_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


