# AppEncryptionDeclarationDocumentResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppEncryptionDeclarationDocument**](AppEncryptionDeclarationDocument.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_encryption_declaration_document_response import AppEncryptionDeclarationDocumentResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppEncryptionDeclarationDocumentResponse from a JSON string
app_encryption_declaration_document_response_instance = AppEncryptionDeclarationDocumentResponse.from_json(json)
# print the JSON string representation of the object
print(AppEncryptionDeclarationDocumentResponse.to_json())

# convert the object into a dict
app_encryption_declaration_document_response_dict = app_encryption_declaration_document_response_instance.to_dict()
# create an instance of AppEncryptionDeclarationDocumentResponse from a dict
app_encryption_declaration_document_response_from_dict = AppEncryptionDeclarationDocumentResponse.from_dict(app_encryption_declaration_document_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


