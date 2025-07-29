# InAppPurchasePriceScheduleCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**InAppPurchasePriceScheduleCreateRequestData**](InAppPurchasePriceScheduleCreateRequestData.md) |  | 
**included** | [**List[InAppPurchasePriceScheduleCreateRequestIncludedInner]**](InAppPurchasePriceScheduleCreateRequestIncludedInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_price_schedule_create_request import InAppPurchasePriceScheduleCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePriceScheduleCreateRequest from a JSON string
in_app_purchase_price_schedule_create_request_instance = InAppPurchasePriceScheduleCreateRequest.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePriceScheduleCreateRequest.to_json())

# convert the object into a dict
in_app_purchase_price_schedule_create_request_dict = in_app_purchase_price_schedule_create_request_instance.to_dict()
# create an instance of InAppPurchasePriceScheduleCreateRequest from a dict
in_app_purchase_price_schedule_create_request_from_dict = InAppPurchasePriceScheduleCreateRequest.from_dict(in_app_purchase_price_schedule_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


