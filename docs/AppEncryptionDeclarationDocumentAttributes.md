# AppEncryptionDeclarationDocumentAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_size** | **int** |  | [optional] 
**file_name** | **str** |  | [optional] 
**asset_token** | **str** |  | [optional] 
**download_url** | **str** |  | [optional] 
**source_file_checksum** | **str** |  | [optional] 
**upload_operations** | [**List[UploadOperation]**](UploadOperation.md) |  | [optional] 
**asset_delivery_state** | [**AppMediaAssetState**](AppMediaAssetState.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_encryption_declaration_document_attributes import AppEncryptionDeclarationDocumentAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppEncryptionDeclarationDocumentAttributes from a JSON string
app_encryption_declaration_document_attributes_instance = AppEncryptionDeclarationDocumentAttributes.from_json(json)
# print the JSON string representation of the object
print(AppEncryptionDeclarationDocumentAttributes.to_json())

# convert the object into a dict
app_encryption_declaration_document_attributes_dict = app_encryption_declaration_document_attributes_instance.to_dict()
# create an instance of AppEncryptionDeclarationDocumentAttributes from a dict
app_encryption_declaration_document_attributes_from_dict = AppEncryptionDeclarationDocumentAttributes.from_dict(app_encryption_declaration_document_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


