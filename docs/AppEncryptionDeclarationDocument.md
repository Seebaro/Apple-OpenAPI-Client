# AppEncryptionDeclarationDocument


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppEncryptionDeclarationDocumentAttributes**](AppEncryptionDeclarationDocumentAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_encryption_declaration_document import AppEncryptionDeclarationDocument

# TODO update the JSON string below
json = "{}"
# create an instance of AppEncryptionDeclarationDocument from a JSON string
app_encryption_declaration_document_instance = AppEncryptionDeclarationDocument.from_json(json)
# print the JSON string representation of the object
print(AppEncryptionDeclarationDocument.to_json())

# convert the object into a dict
app_encryption_declaration_document_dict = app_encryption_declaration_document_instance.to_dict()
# create an instance of AppEncryptionDeclarationDocument from a dict
app_encryption_declaration_document_from_dict = AppEncryptionDeclarationDocument.from_dict(app_encryption_declaration_document_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


