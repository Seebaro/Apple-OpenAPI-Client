# BundleIdCapabilitiesWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BundleIdCapability]**](BundleIdCapability.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.bundle_id_capabilities_without_includes_response import BundleIdCapabilitiesWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BundleIdCapabilitiesWithoutIncludesResponse from a JSON string
bundle_id_capabilities_without_includes_response_instance = BundleIdCapabilitiesWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(BundleIdCapabilitiesWithoutIncludesResponse.to_json())

# convert the object into a dict
bundle_id_capabilities_without_includes_response_dict = bundle_id_capabilities_without_includes_response_instance.to_dict()
# create an instance of BundleIdCapabilitiesWithoutIncludesResponse from a dict
bundle_id_capabilities_without_includes_response_from_dict = BundleIdCapabilitiesWithoutIncludesResponse.from_dict(bundle_id_capabilities_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


