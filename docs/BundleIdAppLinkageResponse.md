# BundleIdAppLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AccessibilityDeclarationCreateRequestDataRelationshipsAppData**](AccessibilityDeclarationCreateRequestDataRelationshipsAppData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.bundle_id_app_linkage_response import BundleIdAppLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BundleIdAppLinkageResponse from a JSON string
bundle_id_app_linkage_response_instance = BundleIdAppLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(BundleIdAppLinkageResponse.to_json())

# convert the object into a dict
bundle_id_app_linkage_response_dict = bundle_id_app_linkage_response_instance.to_dict()
# create an instance of BundleIdAppLinkageResponse from a dict
bundle_id_app_linkage_response_from_dict = BundleIdAppLinkageResponse.from_dict(bundle_id_app_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


