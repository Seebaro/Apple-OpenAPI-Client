# AppEncryptionDeclarationDocumentUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipAdvancedExperienceImageUpdateRequestDataAttributes**](AppClipAdvancedExperienceImageUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_encryption_declaration_document_update_request_data import AppEncryptionDeclarationDocumentUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppEncryptionDeclarationDocumentUpdateRequestData from a JSON string
app_encryption_declaration_document_update_request_data_instance = AppEncryptionDeclarationDocumentUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppEncryptionDeclarationDocumentUpdateRequestData.to_json())

# convert the object into a dict
app_encryption_declaration_document_update_request_data_dict = app_encryption_declaration_document_update_request_data_instance.to_dict()
# create an instance of AppEncryptionDeclarationDocumentUpdateRequestData from a dict
app_encryption_declaration_document_update_request_data_from_dict = AppEncryptionDeclarationDocumentUpdateRequestData.from_dict(app_encryption_declaration_document_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


