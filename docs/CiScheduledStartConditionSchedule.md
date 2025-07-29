# CiScheduledStartConditionSchedule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**frequency** | **str** |  | [optional] 
**days** | **List[str]** |  | [optional] 
**hour** | **int** |  | [optional] 
**minute** | **int** |  | [optional] 
**timezone** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.ci_scheduled_start_condition_schedule import CiScheduledStartConditionSchedule

# TODO update the JSON string below
json = "{}"
# create an instance of CiScheduledStartConditionSchedule from a JSON string
ci_scheduled_start_condition_schedule_instance = CiScheduledStartConditionSchedule.from_json(json)
# print the JSON string representation of the object
print(CiScheduledStartConditionSchedule.to_json())

# convert the object into a dict
ci_scheduled_start_condition_schedule_dict = ci_scheduled_start_condition_schedule_instance.to_dict()
# create an instance of CiScheduledStartConditionSchedule from a dict
ci_scheduled_start_condition_schedule_from_dict = CiScheduledStartConditionSchedule.from_dict(ci_scheduled_start_condition_schedule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


