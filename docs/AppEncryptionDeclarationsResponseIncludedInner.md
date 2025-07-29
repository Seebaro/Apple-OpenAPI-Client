# AppEncryptionDeclarationsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppEncryptionDeclarationDocumentAttributes**](AppEncryptionDeclarationDocumentAttributes.md) |  | [optional] 
**relationships** | [**BuildRelationships**](BuildRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_encryption_declarations_response_included_inner import AppEncryptionDeclarationsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppEncryptionDeclarationsResponseIncludedInner from a JSON string
app_encryption_declarations_response_included_inner_instance = AppEncryptionDeclarationsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppEncryptionDeclarationsResponseIncludedInner.to_json())

# convert the object into a dict
app_encryption_declarations_response_included_inner_dict = app_encryption_declarations_response_included_inner_instance.to_dict()
# create an instance of AppEncryptionDeclarationsResponseIncludedInner from a dict
app_encryption_declarations_response_included_inner_from_dict = AppEncryptionDeclarationsResponseIncludedInner.from_dict(app_encryption_declarations_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


