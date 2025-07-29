# BuildAppStoreVersionLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AlternativeDistributionPackageCreateRequestDataRelationshipsAppStoreVersionData**](AlternativeDistributionPackageCreateRequestDataRelationshipsAppStoreVersionData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.build_app_store_version_linkage_response import BuildAppStoreVersionLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BuildAppStoreVersionLinkageResponse from a JSON string
build_app_store_version_linkage_response_instance = BuildAppStoreVersionLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(BuildAppStoreVersionLinkageResponse.to_json())

# convert the object into a dict
build_app_store_version_linkage_response_dict = build_app_store_version_linkage_response_instance.to_dict()
# create an instance of BuildAppStoreVersionLinkageResponse from a dict
build_app_store_version_linkage_response_from_dict = BuildAppStoreVersionLinkageResponse.from_dict(build_app_store_version_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


