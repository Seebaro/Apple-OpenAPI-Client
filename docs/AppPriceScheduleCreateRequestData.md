# AppPriceScheduleCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**AppPriceScheduleCreateRequestDataRelationships**](AppPriceScheduleCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.app_price_schedule_create_request_data import AppPriceScheduleCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppPriceScheduleCreateRequestData from a JSON string
app_price_schedule_create_request_data_instance = AppPriceScheduleCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppPriceScheduleCreateRequestData.to_json())

# convert the object into a dict
app_price_schedule_create_request_data_dict = app_price_schedule_create_request_data_instance.to_dict()
# create an instance of AppPriceScheduleCreateRequestData from a dict
app_price_schedule_create_request_data_from_dict = AppPriceScheduleCreateRequestData.from_dict(app_price_schedule_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


