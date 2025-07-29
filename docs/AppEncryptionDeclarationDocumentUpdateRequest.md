# AppEncryptionDeclarationDocumentUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppEncryptionDeclarationDocumentUpdateRequestData**](AppEncryptionDeclarationDocumentUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.app_encryption_declaration_document_update_request import AppEncryptionDeclarationDocumentUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppEncryptionDeclarationDocumentUpdateRequest from a JSON string
app_encryption_declaration_document_update_request_instance = AppEncryptionDeclarationDocumentUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(AppEncryptionDeclarationDocumentUpdateRequest.to_json())

# convert the object into a dict
app_encryption_declaration_document_update_request_dict = app_encryption_declaration_document_update_request_instance.to_dict()
# create an instance of AppEncryptionDeclarationDocumentUpdateRequest from a dict
app_encryption_declaration_document_update_request_from_dict = AppEncryptionDeclarationDocumentUpdateRequest.from_dict(app_encryption_declaration_document_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


