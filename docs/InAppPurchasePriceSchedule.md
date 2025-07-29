# InAppPurchasePriceSchedule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**relationships** | [**InAppPurchasePriceScheduleRelationships**](InAppPurchasePriceScheduleRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_price_schedule import InAppPurchasePriceSchedule

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePriceSchedule from a JSON string
in_app_purchase_price_schedule_instance = InAppPurchasePriceSchedule.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePriceSchedule.to_json())

# convert the object into a dict
in_app_purchase_price_schedule_dict = in_app_purchase_price_schedule_instance.to_dict()
# create an instance of InAppPurchasePriceSchedule from a dict
in_app_purchase_price_schedule_from_dict = InAppPurchasePriceSchedule.from_dict(in_app_purchase_price_schedule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


