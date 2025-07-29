# ScmGitReferenceResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ScmGitReference**](ScmGitReference.md) |  | 
**included** | [**List[ScmRepository]**](ScmRepository.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.scm_git_reference_response import ScmGitReferenceResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ScmGitReferenceResponse from a JSON string
scm_git_reference_response_instance = ScmGitReferenceResponse.from_json(json)
# print the JSON string representation of the object
print(ScmGitReferenceResponse.to_json())

# convert the object into a dict
scm_git_reference_response_dict = scm_git_reference_response_instance.to_dict()
# create an instance of ScmGitReferenceResponse from a dict
scm_git_reference_response_from_dict = ScmGitReferenceResponse.from_dict(scm_git_reference_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


