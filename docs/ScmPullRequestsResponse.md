# ScmPullRequestsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[ScmPullRequest]**](ScmPullRequest.md) |  | 
**included** | [**List[ScmRepository]**](ScmRepository.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.scm_pull_requests_response import ScmPullRequestsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ScmPullRequestsResponse from a JSON string
scm_pull_requests_response_instance = ScmPullRequestsResponse.from_json(json)
# print the JSON string representation of the object
print(ScmPullRequestsResponse.to_json())

# convert the object into a dict
scm_pull_requests_response_dict = scm_pull_requests_response_instance.to_dict()
# create an instance of ScmPullRequestsResponse from a dict
scm_pull_requests_response_from_dict = ScmPullRequestsResponse.from_dict(scm_pull_requests_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


