# AppEncryptionDeclarationAppLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AccessibilityDeclarationCreateRequestDataRelationshipsAppData**](AccessibilityDeclarationCreateRequestDataRelationshipsAppData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_encryption_declaration_app_linkage_response import AppEncryptionDeclarationAppLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppEncryptionDeclarationAppLinkageResponse from a JSON string
app_encryption_declaration_app_linkage_response_instance = AppEncryptionDeclarationAppLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppEncryptionDeclarationAppLinkageResponse.to_json())

# convert the object into a dict
app_encryption_declaration_app_linkage_response_dict = app_encryption_declaration_app_linkage_response_instance.to_dict()
# create an instance of AppEncryptionDeclarationAppLinkageResponse from a dict
app_encryption_declaration_app_linkage_response_from_dict = AppEncryptionDeclarationAppLinkageResponse.from_dict(app_encryption_declaration_app_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


