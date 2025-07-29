# ScmPullRequestResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ScmPullRequest**](ScmPullRequest.md) |  | 
**included** | [**List[ScmRepository]**](ScmRepository.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.scm_pull_request_response import ScmPullRequestResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ScmPullRequestResponse from a JSON string
scm_pull_request_response_instance = ScmPullRequestResponse.from_json(json)
# print the JSON string representation of the object
print(ScmPullRequestResponse.to_json())

# convert the object into a dict
scm_pull_request_response_dict = scm_pull_request_response_instance.to_dict()
# create an instance of ScmPullRequestResponse from a dict
scm_pull_request_response_from_dict = ScmPullRequestResponse.from_dict(scm_pull_request_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


