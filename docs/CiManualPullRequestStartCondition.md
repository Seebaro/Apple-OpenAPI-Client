# CiManualPullRequestStartCondition


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | [**CiBranchPatterns**](CiBranchPatterns.md) |  | [optional] 
**destination** | [**CiBranchPatterns**](CiBranchPatterns.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_manual_pull_request_start_condition import CiManualPullRequestStartCondition

# TODO update the JSON string below
json = "{}"
# create an instance of CiManualPullRequestStartCondition from a JSON string
ci_manual_pull_request_start_condition_instance = CiManualPullRequestStartCondition.from_json(json)
# print the JSON string representation of the object
print(CiManualPullRequestStartCondition.to_json())

# convert the object into a dict
ci_manual_pull_request_start_condition_dict = ci_manual_pull_request_start_condition_instance.to_dict()
# create an instance of CiManualPullRequestStartCondition from a dict
ci_manual_pull_request_start_condition_from_dict = CiManualPullRequestStartCondition.from_dict(ci_manual_pull_request_start_condition_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


