# AppEncryptionDeclarationRelationshipsBuilds


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppEncryptionDeclarationRelationshipsBuildsDataInner]**](AppEncryptionDeclarationRelationshipsBuildsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_encryption_declaration_relationships_builds import AppEncryptionDeclarationRelationshipsBuilds

# TODO update the JSON string below
json = "{}"
# create an instance of AppEncryptionDeclarationRelationshipsBuilds from a JSON string
app_encryption_declaration_relationships_builds_instance = AppEncryptionDeclarationRelationshipsBuilds.from_json(json)
# print the JSON string representation of the object
print(AppEncryptionDeclarationRelationshipsBuilds.to_json())

# convert the object into a dict
app_encryption_declaration_relationships_builds_dict = app_encryption_declaration_relationships_builds_instance.to_dict()
# create an instance of AppEncryptionDeclarationRelationshipsBuilds from a dict
app_encryption_declaration_relationships_builds_from_dict = AppEncryptionDeclarationRelationshipsBuilds.from_dict(app_encryption_declaration_relationships_builds_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


