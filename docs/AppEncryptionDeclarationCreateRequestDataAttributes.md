# AppEncryptionDeclarationCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app_description** | **str** |  | 
**contains_proprietary_cryptography** | **bool** |  | 
**contains_third_party_cryptography** | **bool** |  | 
**available_on_french_store** | **bool** |  | 

## Example

```python
from openapi_client.models.app_encryption_declaration_create_request_data_attributes import AppEncryptionDeclarationCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppEncryptionDeclarationCreateRequestDataAttributes from a JSON string
app_encryption_declaration_create_request_data_attributes_instance = AppEncryptionDeclarationCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(AppEncryptionDeclarationCreateRequestDataAttributes.to_json())

# convert the object into a dict
app_encryption_declaration_create_request_data_attributes_dict = app_encryption_declaration_create_request_data_attributes_instance.to_dict()
# create an instance of AppEncryptionDeclarationCreateRequestDataAttributes from a dict
app_encryption_declaration_create_request_data_attributes_from_dict = AppEncryptionDeclarationCreateRequestDataAttributes.from_dict(app_encryption_declaration_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


