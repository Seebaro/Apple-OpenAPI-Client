# CiActionTestConfiguration


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**kind** | **str** |  | [optional] 
**test_plan_name** | **str** |  | [optional] 
**test_destinations** | [**List[CiTestDestination]**](CiTestDestination.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_action_test_configuration import CiActionTestConfiguration

# TODO update the JSON string below
json = "{}"
# create an instance of CiActionTestConfiguration from a JSON string
ci_action_test_configuration_instance = CiActionTestConfiguration.from_json(json)
# print the JSON string representation of the object
print(CiActionTestConfiguration.to_json())

# convert the object into a dict
ci_action_test_configuration_dict = ci_action_test_configuration_instance.to_dict()
# create an instance of CiActionTestConfiguration from a dict
ci_action_test_configuration_from_dict = CiActionTestConfiguration.from_dict(ci_action_test_configuration_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


