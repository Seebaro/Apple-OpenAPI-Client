# ScmPullRequestAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** |  | [optional] 
**number** | **int** |  | [optional] 
**web_url** | **str** |  | [optional] 
**source_repository_owner** | **str** |  | [optional] 
**source_repository_name** | **str** |  | [optional] 
**source_branch_name** | **str** |  | [optional] 
**destination_repository_owner** | **str** |  | [optional] 
**destination_repository_name** | **str** |  | [optional] 
**destination_branch_name** | **str** |  | [optional] 
**is_closed** | **bool** |  | [optional] 
**is_cross_repository** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.scm_pull_request_attributes import ScmPullRequestAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of ScmPullRequestAttributes from a JSON string
scm_pull_request_attributes_instance = ScmPullRequestAttributes.from_json(json)
# print the JSON string representation of the object
print(ScmPullRequestAttributes.to_json())

# convert the object into a dict
scm_pull_request_attributes_dict = scm_pull_request_attributes_instance.to_dict()
# create an instance of ScmPullRequestAttributes from a dict
scm_pull_request_attributes_from_dict = ScmPullRequestAttributes.from_dict(scm_pull_request_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


