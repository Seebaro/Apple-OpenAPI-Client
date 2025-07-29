# CiWorkflowUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CiWorkflowUpdateRequestData**](CiWorkflowUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.ci_workflow_update_request import CiWorkflowUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CiWorkflowUpdateRequest from a JSON string
ci_workflow_update_request_instance = CiWorkflowUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(CiWorkflowUpdateRequest.to_json())

# convert the object into a dict
ci_workflow_update_request_dict = ci_workflow_update_request_instance.to_dict()
# create an instance of CiWorkflowUpdateRequest from a dict
ci_workflow_update_request_from_dict = CiWorkflowUpdateRequest.from_dict(ci_workflow_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


