# ScmRepositoriesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[ScmRepository]**](ScmRepository.md) |  | 
**included** | [**List[ScmRepositoriesResponseIncludedInner]**](ScmRepositoriesResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.scm_repositories_response import ScmRepositoriesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ScmRepositoriesResponse from a JSON string
scm_repositories_response_instance = ScmRepositoriesResponse.from_json(json)
# print the JSON string representation of the object
print(ScmRepositoriesResponse.to_json())

# convert the object into a dict
scm_repositories_response_dict = scm_repositories_response_instance.to_dict()
# create an instance of ScmRepositoriesResponse from a dict
scm_repositories_response_from_dict = ScmRepositoriesResponse.from_dict(scm_repositories_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


