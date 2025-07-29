# AppPriceScheduleResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppPriceSchedule**](AppPriceSchedule.md) |  | 
**included** | [**List[AppPriceScheduleResponseIncludedInner]**](AppPriceScheduleResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_price_schedule_response import AppPriceScheduleResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppPriceScheduleResponse from a JSON string
app_price_schedule_response_instance = AppPriceScheduleResponse.from_json(json)
# print the JSON string representation of the object
print(AppPriceScheduleResponse.to_json())

# convert the object into a dict
app_price_schedule_response_dict = app_price_schedule_response_instance.to_dict()
# create an instance of AppPriceScheduleResponse from a dict
app_price_schedule_response_from_dict = AppPriceScheduleResponse.from_dict(app_price_schedule_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


