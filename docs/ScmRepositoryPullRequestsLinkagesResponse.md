# ScmRepositoryPullRequestsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiBuildRunRelationshipsPullRequestData]**](CiBuildRunRelationshipsPullRequestData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.scm_repository_pull_requests_linkages_response import ScmRepositoryPullRequestsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ScmRepositoryPullRequestsLinkagesResponse from a JSON string
scm_repository_pull_requests_linkages_response_instance = ScmRepositoryPullRequestsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(ScmRepositoryPullRequestsLinkagesResponse.to_json())

# convert the object into a dict
scm_repository_pull_requests_linkages_response_dict = scm_repository_pull_requests_linkages_response_instance.to_dict()
# create an instance of ScmRepositoryPullRequestsLinkagesResponse from a dict
scm_repository_pull_requests_linkages_response_from_dict = ScmRepositoryPullRequestsLinkagesResponse.from_dict(scm_repository_pull_requests_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


