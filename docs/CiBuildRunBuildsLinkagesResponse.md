# CiBuildRunBuildsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppEncryptionDeclarationRelationshipsBuildsDataInner]**](AppEncryptionDeclarationRelationshipsBuildsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_build_run_builds_linkages_response import CiBuildRunBuildsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildRunBuildsLinkagesResponse from a JSON string
ci_build_run_builds_linkages_response_instance = CiBuildRunBuildsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(CiBuildRunBuildsLinkagesResponse.to_json())

# convert the object into a dict
ci_build_run_builds_linkages_response_dict = ci_build_run_builds_linkages_response_instance.to_dict()
# create an instance of CiBuildRunBuildsLinkagesResponse from a dict
ci_build_run_builds_linkages_response_from_dict = CiBuildRunBuildsLinkagesResponse.from_dict(ci_build_run_builds_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


