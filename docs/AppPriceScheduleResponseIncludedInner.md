# AppPriceScheduleResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppPriceV2Attributes**](AppPriceV2Attributes.md) |  | [optional] 
**relationships** | [**AppPriceV2Relationships**](AppPriceV2Relationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_price_schedule_response_included_inner import AppPriceScheduleResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppPriceScheduleResponseIncludedInner from a JSON string
app_price_schedule_response_included_inner_instance = AppPriceScheduleResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppPriceScheduleResponseIncludedInner.to_json())

# convert the object into a dict
app_price_schedule_response_included_inner_dict = app_price_schedule_response_included_inner_instance.to_dict()
# create an instance of AppPriceScheduleResponseIncludedInner from a dict
app_price_schedule_response_included_inner_from_dict = AppPriceScheduleResponseIncludedInner.from_dict(app_price_schedule_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


