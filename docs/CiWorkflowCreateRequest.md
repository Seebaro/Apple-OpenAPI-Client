# CiWorkflowCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CiWorkflowCreateRequestData**](CiWorkflowCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.ci_workflow_create_request import CiWorkflowCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CiWorkflowCreateRequest from a JSON string
ci_workflow_create_request_instance = CiWorkflowCreateRequest.from_json(json)
# print the JSON string representation of the object
print(CiWorkflowCreateRequest.to_json())

# convert the object into a dict
ci_workflow_create_request_dict = ci_workflow_create_request_instance.to_dict()
# create an instance of CiWorkflowCreateRequest from a dict
ci_workflow_create_request_from_dict = CiWorkflowCreateRequest.from_dict(ci_workflow_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


