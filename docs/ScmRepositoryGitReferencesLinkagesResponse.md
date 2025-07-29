# ScmRepositoryGitReferencesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiBuildRunRelationshipsSourceBranchOrTagData]**](CiBuildRunRelationshipsSourceBranchOrTagData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.scm_repository_git_references_linkages_response import ScmRepositoryGitReferencesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ScmRepositoryGitReferencesLinkagesResponse from a JSON string
scm_repository_git_references_linkages_response_instance = ScmRepositoryGitReferencesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(ScmRepositoryGitReferencesLinkagesResponse.to_json())

# convert the object into a dict
scm_repository_git_references_linkages_response_dict = scm_repository_git_references_linkages_response_instance.to_dict()
# create an instance of ScmRepositoryGitReferencesLinkagesResponse from a dict
scm_repository_git_references_linkages_response_from_dict = ScmRepositoryGitReferencesLinkagesResponse.from_dict(scm_repository_git_references_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


