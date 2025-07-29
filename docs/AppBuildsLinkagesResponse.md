# AppBuildsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppEncryptionDeclarationRelationshipsBuildsDataInner]**](AppEncryptionDeclarationRelationshipsBuildsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_builds_linkages_response import AppBuildsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppBuildsLinkagesResponse from a JSON string
app_builds_linkages_response_instance = AppBuildsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppBuildsLinkagesResponse.to_json())

# convert the object into a dict
app_builds_linkages_response_dict = app_builds_linkages_response_instance.to_dict()
# create an instance of AppBuildsLinkagesResponse from a dict
app_builds_linkages_response_from_dict = AppBuildsLinkagesResponse.from_dict(app_builds_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


