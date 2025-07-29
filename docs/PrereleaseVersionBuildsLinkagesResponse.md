# PrereleaseVersionBuildsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppEncryptionDeclarationRelationshipsBuildsDataInner]**](AppEncryptionDeclarationRelationshipsBuildsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.prerelease_version_builds_linkages_response import PrereleaseVersionBuildsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PrereleaseVersionBuildsLinkagesResponse from a JSON string
prerelease_version_builds_linkages_response_instance = PrereleaseVersionBuildsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(PrereleaseVersionBuildsLinkagesResponse.to_json())

# convert the object into a dict
prerelease_version_builds_linkages_response_dict = prerelease_version_builds_linkages_response_instance.to_dict()
# create an instance of PrereleaseVersionBuildsLinkagesResponse from a dict
prerelease_version_builds_linkages_response_from_dict = PrereleaseVersionBuildsLinkagesResponse.from_dict(prerelease_version_builds_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


