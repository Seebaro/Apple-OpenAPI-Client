# AppEventAttributesTerritorySchedulesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**territories** | **List[str]** |  | [optional] 
**publish_start** | **datetime** |  | [optional] 
**event_start** | **datetime** |  | [optional] 
**event_end** | **datetime** |  | [optional] 

## Example

```python
from openapi_client.models.app_event_attributes_territory_schedules_inner import AppEventAttributesTerritorySchedulesInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventAttributesTerritorySchedulesInner from a JSON string
app_event_attributes_territory_schedules_inner_instance = AppEventAttributesTerritorySchedulesInner.from_json(json)
# print the JSON string representation of the object
print(AppEventAttributesTerritorySchedulesInner.to_json())

# convert the object into a dict
app_event_attributes_territory_schedules_inner_dict = app_event_attributes_territory_schedules_inner_instance.to_dict()
# create an instance of AppEventAttributesTerritorySchedulesInner from a dict
app_event_attributes_territory_schedules_inner_from_dict = AppEventAttributesTerritorySchedulesInner.from_dict(app_event_attributes_territory_schedules_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


