# ScmGitReferencesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[ScmGitReference]**](ScmGitReference.md) |  | 
**included** | [**List[ScmRepository]**](ScmRepository.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.scm_git_references_response import ScmGitReferencesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ScmGitReferencesResponse from a JSON string
scm_git_references_response_instance = ScmGitReferencesResponse.from_json(json)
# print the JSON string representation of the object
print(ScmGitReferencesResponse.to_json())

# convert the object into a dict
scm_git_references_response_dict = scm_git_references_response_instance.to_dict()
# create an instance of ScmGitReferencesResponse from a dict
scm_git_references_response_from_dict = ScmGitReferencesResponse.from_dict(scm_git_references_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


