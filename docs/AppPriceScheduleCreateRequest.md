# AppPriceScheduleCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppPriceScheduleCreateRequestData**](AppPriceScheduleCreateRequestData.md) |  | 
**included** | [**List[AppPriceScheduleCreateRequestIncludedInner]**](AppPriceScheduleCreateRequestIncludedInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_price_schedule_create_request import AppPriceScheduleCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppPriceScheduleCreateRequest from a JSON string
app_price_schedule_create_request_instance = AppPriceScheduleCreateRequest.from_json(json)
# print the JSON string representation of the object
print(AppPriceScheduleCreateRequest.to_json())

# convert the object into a dict
app_price_schedule_create_request_dict = app_price_schedule_create_request_instance.to_dict()
# create an instance of AppPriceScheduleCreateRequest from a dict
app_price_schedule_create_request_from_dict = AppPriceScheduleCreateRequest.from_dict(app_price_schedule_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


