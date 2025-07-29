# AppEventAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | [optional] 
**badge** | **str** |  | [optional] 
**event_state** | **str** |  | [optional] 
**deep_link** | **str** |  | [optional] 
**purchase_requirement** | **str** |  | [optional] 
**primary_locale** | **str** |  | [optional] 
**priority** | **str** |  | [optional] 
**purpose** | **str** |  | [optional] 
**territory_schedules** | [**List[AppEventAttributesTerritorySchedulesInner]**](AppEventAttributesTerritorySchedulesInner.md) |  | [optional] 
**archived_territory_schedules** | [**List[AppEventAttributesTerritorySchedulesInner]**](AppEventAttributesTerritorySchedulesInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_attributes import AppEventAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventAttributes from a JSON string
app_event_attributes_instance = AppEventAttributes.from_json(json)
# print the JSON string representation of the object
print(AppEventAttributes.to_json())

# convert the object into a dict
app_event_attributes_dict = app_event_attributes_instance.to_dict()
# create an instance of AppEventAttributes from a dict
app_event_attributes_from_dict = AppEventAttributes.from_dict(app_event_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


