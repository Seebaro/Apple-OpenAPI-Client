# BuildPreReleaseVersionLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppRelationshipsPreReleaseVersionsDataInner**](AppRelationshipsPreReleaseVersionsDataInner.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.build_pre_release_version_linkage_response import BuildPreReleaseVersionLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BuildPreReleaseVersionLinkageResponse from a JSON string
build_pre_release_version_linkage_response_instance = BuildPreReleaseVersionLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(BuildPreReleaseVersionLinkageResponse.to_json())

# convert the object into a dict
build_pre_release_version_linkage_response_dict = build_pre_release_version_linkage_response_instance.to_dict()
# create an instance of BuildPreReleaseVersionLinkageResponse from a dict
build_pre_release_version_linkage_response_from_dict = BuildPreReleaseVersionLinkageResponse.from_dict(build_pre_release_version_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


