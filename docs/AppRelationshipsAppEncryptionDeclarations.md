# AppRelationshipsAppEncryptionDeclarations


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppEncryptionDeclarationDocumentCreateRequestDataRelationshipsAppEncryptionDeclarationData]**](AppEncryptionDeclarationDocumentCreateRequestDataRelationshipsAppEncryptionDeclarationData.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_relationships_app_encryption_declarations import AppRelationshipsAppEncryptionDeclarations

# TODO update the JSON string below
json = "{}"
# create an instance of AppRelationshipsAppEncryptionDeclarations from a JSON string
app_relationships_app_encryption_declarations_instance = AppRelationshipsAppEncryptionDeclarations.from_json(json)
# print the JSON string representation of the object
print(AppRelationshipsAppEncryptionDeclarations.to_json())

# convert the object into a dict
app_relationships_app_encryption_declarations_dict = app_relationships_app_encryption_declarations_instance.to_dict()
# create an instance of AppRelationshipsAppEncryptionDeclarations from a dict
app_relationships_app_encryption_declarations_from_dict = AppRelationshipsAppEncryptionDeclarations.from_dict(app_relationships_app_encryption_declarations_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


