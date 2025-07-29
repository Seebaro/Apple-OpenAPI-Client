# BetaGroupAppLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AccessibilityDeclarationCreateRequestDataRelationshipsAppData**](AccessibilityDeclarationCreateRequestDataRelationshipsAppData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.beta_group_app_linkage_response import BetaGroupAppLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaGroupAppLinkageResponse from a JSON string
beta_group_app_linkage_response_instance = BetaGroupAppLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(BetaGroupAppLinkageResponse.to_json())

# convert the object into a dict
beta_group_app_linkage_response_dict = beta_group_app_linkage_response_instance.to_dict()
# create an instance of BetaGroupAppLinkageResponse from a dict
beta_group_app_linkage_response_from_dict = BetaGroupAppLinkageResponse.from_dict(beta_group_app_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


