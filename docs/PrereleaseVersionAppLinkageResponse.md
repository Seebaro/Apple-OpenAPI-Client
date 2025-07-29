# PrereleaseVersionAppLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AccessibilityDeclarationCreateRequestDataRelationshipsAppData**](AccessibilityDeclarationCreateRequestDataRelationshipsAppData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.prerelease_version_app_linkage_response import PrereleaseVersionAppLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PrereleaseVersionAppLinkageResponse from a JSON string
prerelease_version_app_linkage_response_instance = PrereleaseVersionAppLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(PrereleaseVersionAppLinkageResponse.to_json())

# convert the object into a dict
prerelease_version_app_linkage_response_dict = prerelease_version_app_linkage_response_instance.to_dict()
# create an instance of PrereleaseVersionAppLinkageResponse from a dict
prerelease_version_app_linkage_response_from_dict = PrereleaseVersionAppLinkageResponse.from_dict(prerelease_version_app_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


