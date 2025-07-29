# BuildAppLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AccessibilityDeclarationCreateRequestDataRelationshipsAppData**](AccessibilityDeclarationCreateRequestDataRelationshipsAppData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.build_app_linkage_response import BuildAppLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BuildAppLinkageResponse from a JSON string
build_app_linkage_response_instance = BuildAppLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(BuildAppLinkageResponse.to_json())

# convert the object into a dict
build_app_linkage_response_dict = build_app_linkage_response_instance.to_dict()
# create an instance of BuildAppLinkageResponse from a dict
build_app_linkage_response_from_dict = BuildAppLinkageResponse.from_dict(build_app_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


