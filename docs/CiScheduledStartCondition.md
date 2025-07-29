# CiScheduledStartCondition


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | [**CiBranchPatterns**](CiBranchPatterns.md) |  | [optional] 
**schedule** | [**CiScheduledStartConditionSchedule**](CiScheduledStartConditionSchedule.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_scheduled_start_condition import CiScheduledStartCondition

# TODO update the JSON string below
json = "{}"
# create an instance of CiScheduledStartCondition from a JSON string
ci_scheduled_start_condition_instance = CiScheduledStartCondition.from_json(json)
# print the JSON string representation of the object
print(CiScheduledStartCondition.to_json())

# convert the object into a dict
ci_scheduled_start_condition_dict = ci_scheduled_start_condition_instance.to_dict()
# create an instance of CiScheduledStartCondition from a dict
ci_scheduled_start_condition_from_dict = CiScheduledStartCondition.from_dict(ci_scheduled_start_condition_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


