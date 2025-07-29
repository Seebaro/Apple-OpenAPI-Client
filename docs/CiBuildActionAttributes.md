# CiBuildActionAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**action_type** | [**CiActionType**](CiActionType.md) |  | [optional] 
**started_date** | **datetime** |  | [optional] 
**finished_date** | **datetime** |  | [optional] 
**issue_counts** | [**CiIssueCounts**](CiIssueCounts.md) |  | [optional] 
**execution_progress** | [**CiExecutionProgress**](CiExecutionProgress.md) |  | [optional] 
**completion_status** | [**CiCompletionStatus**](CiCompletionStatus.md) |  | [optional] 
**is_required_to_pass** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.ci_build_action_attributes import CiBuildActionAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildActionAttributes from a JSON string
ci_build_action_attributes_instance = CiBuildActionAttributes.from_json(json)
# print the JSON string representation of the object
print(CiBuildActionAttributes.to_json())

# convert the object into a dict
ci_build_action_attributes_dict = ci_build_action_attributes_instance.to_dict()
# create an instance of CiBuildActionAttributes from a dict
ci_build_action_attributes_from_dict = CiBuildActionAttributes.from_dict(ci_build_action_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


