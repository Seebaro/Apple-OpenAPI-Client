# ProfileBundleIdLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BundleIdCapabilityCreateRequestDataRelationshipsBundleIdData**](BundleIdCapabilityCreateRequestDataRelationshipsBundleIdData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.profile_bundle_id_linkage_response import ProfileBundleIdLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ProfileBundleIdLinkageResponse from a JSON string
profile_bundle_id_linkage_response_instance = ProfileBundleIdLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(ProfileBundleIdLinkageResponse.to_json())

# convert the object into a dict
profile_bundle_id_linkage_response_dict = profile_bundle_id_linkage_response_instance.to_dict()
# create an instance of ProfileBundleIdLinkageResponse from a dict
profile_bundle_id_linkage_response_from_dict = ProfileBundleIdLinkageResponse.from_dict(profile_bundle_id_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


