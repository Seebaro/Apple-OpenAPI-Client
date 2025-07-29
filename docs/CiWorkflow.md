# CiWorkflow


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**CiWorkflowAttributes**](CiWorkflowAttributes.md) |  | [optional] 
**relationships** | [**CiWorkflowRelationships**](CiWorkflowRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_workflow import CiWorkflow

# TODO update the JSON string below
json = "{}"
# create an instance of CiWorkflow from a JSON string
ci_workflow_instance = CiWorkflow.from_json(json)
# print the JSON string representation of the object
print(CiWorkflow.to_json())

# convert the object into a dict
ci_workflow_dict = ci_workflow_instance.to_dict()
# create an instance of CiWorkflow from a dict
ci_workflow_from_dict = CiWorkflow.from_dict(ci_workflow_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


