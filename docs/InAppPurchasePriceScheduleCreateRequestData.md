# InAppPurchasePriceScheduleCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**InAppPurchasePriceScheduleCreateRequestDataRelationships**](InAppPurchasePriceScheduleCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_price_schedule_create_request_data import InAppPurchasePriceScheduleCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePriceScheduleCreateRequestData from a JSON string
in_app_purchase_price_schedule_create_request_data_instance = InAppPurchasePriceScheduleCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePriceScheduleCreateRequestData.to_json())

# convert the object into a dict
in_app_purchase_price_schedule_create_request_data_dict = in_app_purchase_price_schedule_create_request_data_instance.to_dict()
# create an instance of InAppPurchasePriceScheduleCreateRequestData from a dict
in_app_purchase_price_schedule_create_request_data_from_dict = InAppPurchasePriceScheduleCreateRequestData.from_dict(in_app_purchase_price_schedule_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


