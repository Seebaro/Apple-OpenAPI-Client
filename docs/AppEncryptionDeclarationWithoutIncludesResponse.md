# AppEncryptionDeclarationWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppEncryptionDeclaration**](AppEncryptionDeclaration.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_encryption_declaration_without_includes_response import AppEncryptionDeclarationWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppEncryptionDeclarationWithoutIncludesResponse from a JSON string
app_encryption_declaration_without_includes_response_instance = AppEncryptionDeclarationWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(AppEncryptionDeclarationWithoutIncludesResponse.to_json())

# convert the object into a dict
app_encryption_declaration_without_includes_response_dict = app_encryption_declaration_without_includes_response_instance.to_dict()
# create an instance of AppEncryptionDeclarationWithoutIncludesResponse from a dict
app_encryption_declaration_without_includes_response_from_dict = AppEncryptionDeclarationWithoutIncludesResponse.from_dict(app_encryption_declaration_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


