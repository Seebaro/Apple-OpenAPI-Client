# CiWorkflowCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**CiWorkflowCreateRequestDataAttributes**](CiWorkflowCreateRequestDataAttributes.md) |  | 
**relationships** | [**CiWorkflowCreateRequestDataRelationships**](CiWorkflowCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.ci_workflow_create_request_data import CiWorkflowCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of CiWorkflowCreateRequestData from a JSON string
ci_workflow_create_request_data_instance = CiWorkflowCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(CiWorkflowCreateRequestData.to_json())

# convert the object into a dict
ci_workflow_create_request_data_dict = ci_workflow_create_request_data_instance.to_dict()
# create an instance of CiWorkflowCreateRequestData from a dict
ci_workflow_create_request_data_from_dict = CiWorkflowCreateRequestData.from_dict(ci_workflow_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


