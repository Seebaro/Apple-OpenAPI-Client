# CiWorkflowCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**description** | **str** |  | 
**branch_start_condition** | [**CiBranchStartCondition**](CiBranchStartCondition.md) |  | [optional] 
**tag_start_condition** | [**CiTagStartCondition**](CiTagStartCondition.md) |  | [optional] 
**pull_request_start_condition** | [**CiPullRequestStartCondition**](CiPullRequestStartCondition.md) |  | [optional] 
**scheduled_start_condition** | [**CiScheduledStartCondition**](CiScheduledStartCondition.md) |  | [optional] 
**manual_branch_start_condition** | [**CiManualBranchStartCondition**](CiManualBranchStartCondition.md) |  | [optional] 
**manual_tag_start_condition** | [**CiManualTagStartCondition**](CiManualTagStartCondition.md) |  | [optional] 
**manual_pull_request_start_condition** | [**CiManualPullRequestStartCondition**](CiManualPullRequestStartCondition.md) |  | [optional] 
**actions** | [**List[CiAction]**](CiAction.md) |  | 
**is_enabled** | **bool** |  | 
**is_locked_for_editing** | **bool** |  | [optional] 
**clean** | **bool** |  | 
**container_file_path** | **str** |  | 

## Example

```python
from openapi_client.models.ci_workflow_create_request_data_attributes import CiWorkflowCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of CiWorkflowCreateRequestDataAttributes from a JSON string
ci_workflow_create_request_data_attributes_instance = CiWorkflowCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(CiWorkflowCreateRequestDataAttributes.to_json())

# convert the object into a dict
ci_workflow_create_request_data_attributes_dict = ci_workflow_create_request_data_attributes_instance.to_dict()
# create an instance of CiWorkflowCreateRequestDataAttributes from a dict
ci_workflow_create_request_data_attributes_from_dict = CiWorkflowCreateRequestDataAttributes.from_dict(ci_workflow_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


