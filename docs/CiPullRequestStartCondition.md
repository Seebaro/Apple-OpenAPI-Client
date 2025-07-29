# CiPullRequestStartCondition


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | [**CiBranchPatterns**](CiBranchPatterns.md) |  | [optional] 
**destination** | [**CiBranchPatterns**](CiBranchPatterns.md) |  | [optional] 
**files_and_folders_rule** | [**CiFilesAndFoldersRule**](CiFilesAndFoldersRule.md) |  | [optional] 
**auto_cancel** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.ci_pull_request_start_condition import CiPullRequestStartCondition

# TODO update the JSON string below
json = "{}"
# create an instance of CiPullRequestStartCondition from a JSON string
ci_pull_request_start_condition_instance = CiPullRequestStartCondition.from_json(json)
# print the JSON string representation of the object
print(CiPullRequestStartCondition.to_json())

# convert the object into a dict
ci_pull_request_start_condition_dict = ci_pull_request_start_condition_instance.to_dict()
# create an instance of CiPullRequestStartCondition from a dict
ci_pull_request_start_condition_from_dict = CiPullRequestStartCondition.from_dict(ci_pull_request_start_condition_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


