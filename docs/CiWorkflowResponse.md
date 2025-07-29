# CiWorkflowResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CiWorkflow**](CiWorkflow.md) |  | 
**included** | [**List[CiWorkflowsResponseIncludedInner]**](CiWorkflowsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.ci_workflow_response import CiWorkflowResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiWorkflowResponse from a JSON string
ci_workflow_response_instance = CiWorkflowResponse.from_json(json)
# print the JSON string representation of the object
print(CiWorkflowResponse.to_json())

# convert the object into a dict
ci_workflow_response_dict = ci_workflow_response_instance.to_dict()
# create an instance of CiWorkflowResponse from a dict
ci_workflow_response_from_dict = CiWorkflowResponse.from_dict(ci_workflow_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


