# BetaAppLocalizationAppLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AccessibilityDeclarationCreateRequestDataRelationshipsAppData**](AccessibilityDeclarationCreateRequestDataRelationshipsAppData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.beta_app_localization_app_linkage_response import BetaAppLocalizationAppLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaAppLocalizationAppLinkageResponse from a JSON string
beta_app_localization_app_linkage_response_instance = BetaAppLocalizationAppLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(BetaAppLocalizationAppLinkageResponse.to_json())

# convert the object into a dict
beta_app_localization_app_linkage_response_dict = beta_app_localization_app_linkage_response_instance.to_dict()
# create an instance of BetaAppLocalizationAppLinkageResponse from a dict
beta_app_localization_app_linkage_response_from_dict = BetaAppLocalizationAppLinkageResponse.from_dict(beta_app_localization_app_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


