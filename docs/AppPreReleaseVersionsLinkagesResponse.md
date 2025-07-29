# AppPreReleaseVersionsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppRelationshipsPreReleaseVersionsDataInner]**](AppRelationshipsPreReleaseVersionsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_pre_release_versions_linkages_response import AppPreReleaseVersionsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppPreReleaseVersionsLinkagesResponse from a JSON string
app_pre_release_versions_linkages_response_instance = AppPreReleaseVersionsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppPreReleaseVersionsLinkagesResponse.to_json())

# convert the object into a dict
app_pre_release_versions_linkages_response_dict = app_pre_release_versions_linkages_response_instance.to_dict()
# create an instance of AppPreReleaseVersionsLinkagesResponse from a dict
app_pre_release_versions_linkages_response_from_dict = AppPreReleaseVersionsLinkagesResponse.from_dict(app_pre_release_versions_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


