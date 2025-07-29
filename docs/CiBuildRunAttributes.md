# CiBuildRunAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**number** | **int** |  | [optional] 
**created_date** | **datetime** |  | [optional] 
**started_date** | **datetime** |  | [optional] 
**finished_date** | **datetime** |  | [optional] 
**source_commit** | [**CiBuildRunAttributesSourceCommit**](CiBuildRunAttributesSourceCommit.md) |  | [optional] 
**destination_commit** | [**CiBuildRunAttributesSourceCommit**](CiBuildRunAttributesSourceCommit.md) |  | [optional] 
**is_pull_request_build** | **bool** |  | [optional] 
**issue_counts** | [**CiIssueCounts**](CiIssueCounts.md) |  | [optional] 
**execution_progress** | [**CiExecutionProgress**](CiExecutionProgress.md) |  | [optional] 
**completion_status** | [**CiCompletionStatus**](CiCompletionStatus.md) |  | [optional] 
**start_reason** | **str** |  | [optional] 
**cancel_reason** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.ci_build_run_attributes import CiBuildRunAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildRunAttributes from a JSON string
ci_build_run_attributes_instance = CiBuildRunAttributes.from_json(json)
# print the JSON string representation of the object
print(CiBuildRunAttributes.to_json())

# convert the object into a dict
ci_build_run_attributes_dict = ci_build_run_attributes_instance.to_dict()
# create an instance of CiBuildRunAttributes from a dict
ci_build_run_attributes_from_dict = CiBuildRunAttributes.from_dict(ci_build_run_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


