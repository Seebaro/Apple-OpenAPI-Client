# AppEncryptionDeclarationCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppEncryptionDeclarationCreateRequestData**](AppEncryptionDeclarationCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.app_encryption_declaration_create_request import AppEncryptionDeclarationCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppEncryptionDeclarationCreateRequest from a JSON string
app_encryption_declaration_create_request_instance = AppEncryptionDeclarationCreateRequest.from_json(json)
# print the JSON string representation of the object
print(AppEncryptionDeclarationCreateRequest.to_json())

# convert the object into a dict
app_encryption_declaration_create_request_dict = app_encryption_declaration_create_request_instance.to_dict()
# create an instance of AppEncryptionDeclarationCreateRequest from a dict
app_encryption_declaration_create_request_from_dict = AppEncryptionDeclarationCreateRequest.from_dict(app_encryption_declaration_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


