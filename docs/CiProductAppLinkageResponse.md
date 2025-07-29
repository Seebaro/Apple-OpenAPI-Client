# CiProductAppLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AccessibilityDeclarationCreateRequestDataRelationshipsAppData**](AccessibilityDeclarationCreateRequestDataRelationshipsAppData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.ci_product_app_linkage_response import CiProductAppLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiProductAppLinkageResponse from a JSON string
ci_product_app_linkage_response_instance = CiProductAppLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(CiProductAppLinkageResponse.to_json())

# convert the object into a dict
ci_product_app_linkage_response_dict = ci_product_app_linkage_response_instance.to_dict()
# create an instance of CiProductAppLinkageResponse from a dict
ci_product_app_linkage_response_from_dict = CiProductAppLinkageResponse.from_dict(ci_product_app_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


