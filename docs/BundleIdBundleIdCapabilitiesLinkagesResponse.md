# BundleIdBundleIdCapabilitiesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BundleIdRelationshipsBundleIdCapabilitiesDataInner]**](BundleIdRelationshipsBundleIdCapabilitiesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.bundle_id_bundle_id_capabilities_linkages_response import BundleIdBundleIdCapabilitiesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BundleIdBundleIdCapabilitiesLinkagesResponse from a JSON string
bundle_id_bundle_id_capabilities_linkages_response_instance = BundleIdBundleIdCapabilitiesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(BundleIdBundleIdCapabilitiesLinkagesResponse.to_json())

# convert the object into a dict
bundle_id_bundle_id_capabilities_linkages_response_dict = bundle_id_bundle_id_capabilities_linkages_response_instance.to_dict()
# create an instance of BundleIdBundleIdCapabilitiesLinkagesResponse from a dict
bundle_id_bundle_id_capabilities_linkages_response_from_dict = BundleIdBundleIdCapabilitiesLinkagesResponse.from_dict(bundle_id_bundle_id_capabilities_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


