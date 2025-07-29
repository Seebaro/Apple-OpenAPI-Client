# CiWorkflowsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiWorkflow]**](CiWorkflow.md) |  | 
**included** | [**List[CiWorkflowsResponseIncludedInner]**](CiWorkflowsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_workflows_response import CiWorkflowsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiWorkflowsResponse from a JSON string
ci_workflows_response_instance = CiWorkflowsResponse.from_json(json)
# print the JSON string representation of the object
print(CiWorkflowsResponse.to_json())

# convert the object into a dict
ci_workflows_response_dict = ci_workflows_response_instance.to_dict()
# create an instance of CiWorkflowsResponse from a dict
ci_workflows_response_from_dict = CiWorkflowsResponse.from_dict(ci_workflows_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


