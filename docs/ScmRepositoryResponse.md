# ScmRepositoryResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ScmRepository**](ScmRepository.md) |  | 
**included** | [**List[ScmRepositoriesResponseIncludedInner]**](ScmRepositoriesResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.scm_repository_response import ScmRepositoryResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ScmRepositoryResponse from a JSON string
scm_repository_response_instance = ScmRepositoryResponse.from_json(json)
# print the JSON string representation of the object
print(ScmRepositoryResponse.to_json())

# convert the object into a dict
scm_repository_response_dict = scm_repository_response_instance.to_dict()
# create an instance of ScmRepositoryResponse from a dict
scm_repository_response_from_dict = ScmRepositoryResponse.from_dict(scm_repository_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


