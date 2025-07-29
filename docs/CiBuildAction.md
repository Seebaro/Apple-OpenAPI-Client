# CiBuildAction


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**CiBuildActionAttributes**](CiBuildActionAttributes.md) |  | [optional] 
**relationships** | [**CiBuildActionRelationships**](CiBuildActionRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_build_action import CiBuildAction

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildAction from a JSON string
ci_build_action_instance = CiBuildAction.from_json(json)
# print the JSON string representation of the object
print(CiBuildAction.to_json())

# convert the object into a dict
ci_build_action_dict = ci_build_action_instance.to_dict()
# create an instance of CiBuildAction from a dict
ci_build_action_from_dict = CiBuildAction.from_dict(ci_build_action_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


