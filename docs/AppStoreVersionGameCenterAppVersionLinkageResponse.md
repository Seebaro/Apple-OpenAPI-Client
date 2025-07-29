# AppStoreVersionGameCenterAppVersionLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppStoreVersionRelationshipsGameCenterAppVersionData**](AppStoreVersionRelationshipsGameCenterAppVersionData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_game_center_app_version_linkage_response import AppStoreVersionGameCenterAppVersionLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionGameCenterAppVersionLinkageResponse from a JSON string
app_store_version_game_center_app_version_linkage_response_instance = AppStoreVersionGameCenterAppVersionLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionGameCenterAppVersionLinkageResponse.to_json())

# convert the object into a dict
app_store_version_game_center_app_version_linkage_response_dict = app_store_version_game_center_app_version_linkage_response_instance.to_dict()
# create an instance of AppStoreVersionGameCenterAppVersionLinkageResponse from a dict
app_store_version_game_center_app_version_linkage_response_from_dict = AppStoreVersionGameCenterAppVersionLinkageResponse.from_dict(app_store_version_game_center_app_version_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


