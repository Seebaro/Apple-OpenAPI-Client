# InAppPurchasePriceScheduleResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**InAppPurchasePriceSchedule**](InAppPurchasePriceSchedule.md) |  | 
**included** | [**List[InAppPurchasePriceScheduleResponseIncludedInner]**](InAppPurchasePriceScheduleResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_price_schedule_response import InAppPurchasePriceScheduleResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePriceScheduleResponse from a JSON string
in_app_purchase_price_schedule_response_instance = InAppPurchasePriceScheduleResponse.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePriceScheduleResponse.to_json())

# convert the object into a dict
in_app_purchase_price_schedule_response_dict = in_app_purchase_price_schedule_response_instance.to_dict()
# create an instance of InAppPurchasePriceScheduleResponse from a dict
in_app_purchase_price_schedule_response_from_dict = InAppPurchasePriceScheduleResponse.from_dict(in_app_purchase_price_schedule_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


