# CiAction


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**action_type** | [**CiActionType**](CiActionType.md) |  | [optional] 
**destination** | **str** |  | [optional] 
**build_distribution_audience** | [**BuildAudienceType**](BuildAudienceType.md) |  | [optional] 
**test_configuration** | [**CiActionTestConfiguration**](CiActionTestConfiguration.md) |  | [optional] 
**scheme** | **str** |  | [optional] 
**platform** | **str** |  | [optional] 
**is_required_to_pass** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.ci_action import CiAction

# TODO update the JSON string below
json = "{}"
# create an instance of CiAction from a JSON string
ci_action_instance = CiAction.from_json(json)
# print the JSON string representation of the object
print(CiAction.to_json())

# convert the object into a dict
ci_action_dict = ci_action_instance.to_dict()
# create an instance of CiAction from a dict
ci_action_from_dict = CiAction.from_dict(ci_action_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


