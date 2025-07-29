# GameCenterAppVersionAppStoreVersionLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AlternativeDistributionPackageCreateRequestDataRelationshipsAppStoreVersionData**](AlternativeDistributionPackageCreateRequestDataRelationshipsAppStoreVersionData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_app_version_app_store_version_linkage_response import GameCenterAppVersionAppStoreVersionLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAppVersionAppStoreVersionLinkageResponse from a JSON string
game_center_app_version_app_store_version_linkage_response_instance = GameCenterAppVersionAppStoreVersionLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterAppVersionAppStoreVersionLinkageResponse.to_json())

# convert the object into a dict
game_center_app_version_app_store_version_linkage_response_dict = game_center_app_version_app_store_version_linkage_response_instance.to_dict()
# create an instance of GameCenterAppVersionAppStoreVersionLinkageResponse from a dict
game_center_app_version_app_store_version_linkage_response_from_dict = GameCenterAppVersionAppStoreVersionLinkageResponse.from_dict(game_center_app_version_app_store_version_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


