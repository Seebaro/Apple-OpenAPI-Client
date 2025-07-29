# CiWorkflowsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**CiMacOsVersionAttributes**](CiMacOsVersionAttributes.md) |  | [optional] 
**relationships** | [**CiMacOsVersionRelationships**](CiMacOsVersionRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_workflows_response_included_inner import CiWorkflowsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of CiWorkflowsResponseIncludedInner from a JSON string
ci_workflows_response_included_inner_instance = CiWorkflowsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(CiWorkflowsResponseIncludedInner.to_json())

# convert the object into a dict
ci_workflows_response_included_inner_dict = ci_workflows_response_included_inner_instance.to_dict()
# create an instance of CiWorkflowsResponseIncludedInner from a dict
ci_workflows_response_included_inner_from_dict = CiWorkflowsResponseIncludedInner.from_dict(ci_workflows_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


