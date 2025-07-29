# AppEncryptionDeclarationDocumentCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppClipAdvancedExperienceImageCreateRequestDataAttributes**](AppClipAdvancedExperienceImageCreateRequestDataAttributes.md) |  | 
**relationships** | [**AppEncryptionDeclarationDocumentCreateRequestDataRelationships**](AppEncryptionDeclarationDocumentCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.app_encryption_declaration_document_create_request_data import AppEncryptionDeclarationDocumentCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppEncryptionDeclarationDocumentCreateRequestData from a JSON string
app_encryption_declaration_document_create_request_data_instance = AppEncryptionDeclarationDocumentCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppEncryptionDeclarationDocumentCreateRequestData.to_json())

# convert the object into a dict
app_encryption_declaration_document_create_request_data_dict = app_encryption_declaration_document_create_request_data_instance.to_dict()
# create an instance of AppEncryptionDeclarationDocumentCreateRequestData from a dict
app_encryption_declaration_document_create_request_data_from_dict = AppEncryptionDeclarationDocumentCreateRequestData.from_dict(app_encryption_declaration_document_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


