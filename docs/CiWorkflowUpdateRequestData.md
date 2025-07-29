# CiWorkflowUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**CiWorkflowUpdateRequestDataAttributes**](CiWorkflowUpdateRequestDataAttributes.md) |  | [optional] 
**relationships** | [**CiWorkflowUpdateRequestDataRelationships**](CiWorkflowUpdateRequestDataRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_workflow_update_request_data import CiWorkflowUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of CiWorkflowUpdateRequestData from a JSON string
ci_workflow_update_request_data_instance = CiWorkflowUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(CiWorkflowUpdateRequestData.to_json())

# convert the object into a dict
ci_workflow_update_request_data_dict = ci_workflow_update_request_data_instance.to_dict()
# create an instance of CiWorkflowUpdateRequestData from a dict
ci_workflow_update_request_data_from_dict = CiWorkflowUpdateRequestData.from_dict(ci_workflow_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


