# ScmPullRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**ScmPullRequestAttributes**](ScmPullRequestAttributes.md) |  | [optional] 
**relationships** | [**ScmGitReferenceRelationships**](ScmGitReferenceRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.scm_pull_request import ScmPullRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ScmPullRequest from a JSON string
scm_pull_request_instance = ScmPullRequest.from_json(json)
# print the JSON string representation of the object
print(ScmPullRequest.to_json())

# convert the object into a dict
scm_pull_request_dict = scm_pull_request_instance.to_dict()
# create an instance of ScmPullRequest from a dict
scm_pull_request_from_dict = ScmPullRequest.from_dict(scm_pull_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


