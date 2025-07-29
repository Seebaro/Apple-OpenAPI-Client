# AppAppEncryptionDeclarationsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppEncryptionDeclarationDocumentCreateRequestDataRelationshipsAppEncryptionDeclarationData]**](AppEncryptionDeclarationDocumentCreateRequestDataRelationshipsAppEncryptionDeclarationData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_app_encryption_declarations_linkages_response import AppAppEncryptionDeclarationsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppAppEncryptionDeclarationsLinkagesResponse from a JSON string
app_app_encryption_declarations_linkages_response_instance = AppAppEncryptionDeclarationsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppAppEncryptionDeclarationsLinkagesResponse.to_json())

# convert the object into a dict
app_app_encryption_declarations_linkages_response_dict = app_app_encryption_declarations_linkages_response_instance.to_dict()
# create an instance of AppAppEncryptionDeclarationsLinkagesResponse from a dict
app_app_encryption_declarations_linkages_response_from_dict = AppAppEncryptionDeclarationsLinkagesResponse.from_dict(app_app_encryption_declarations_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


