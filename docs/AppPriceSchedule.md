# AppPriceSchedule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**relationships** | [**AppPriceScheduleRelationships**](AppPriceScheduleRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_price_schedule import AppPriceSchedule

# TODO update the JSON string below
json = "{}"
# create an instance of AppPriceSchedule from a JSON string
app_price_schedule_instance = AppPriceSchedule.from_json(json)
# print the JSON string representation of the object
print(AppPriceSchedule.to_json())

# convert the object into a dict
app_price_schedule_dict = app_price_schedule_instance.to_dict()
# create an instance of AppPriceSchedule from a dict
app_price_schedule_from_dict = AppPriceSchedule.from_dict(app_price_schedule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


