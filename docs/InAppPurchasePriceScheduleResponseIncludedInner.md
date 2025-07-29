# InAppPurchasePriceScheduleResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**InAppPurchasePriceAttributes**](InAppPurchasePriceAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 
**relationships** | [**InAppPurchasePriceRelationships**](InAppPurchasePriceRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_price_schedule_response_included_inner import InAppPurchasePriceScheduleResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePriceScheduleResponseIncludedInner from a JSON string
in_app_purchase_price_schedule_response_included_inner_instance = InAppPurchasePriceScheduleResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePriceScheduleResponseIncludedInner.to_json())

# convert the object into a dict
in_app_purchase_price_schedule_response_included_inner_dict = in_app_purchase_price_schedule_response_included_inner_instance.to_dict()
# create an instance of InAppPurchasePriceScheduleResponseIncludedInner from a dict
in_app_purchase_price_schedule_response_included_inner_from_dict = InAppPurchasePriceScheduleResponseIncludedInner.from_dict(in_app_purchase_price_schedule_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


