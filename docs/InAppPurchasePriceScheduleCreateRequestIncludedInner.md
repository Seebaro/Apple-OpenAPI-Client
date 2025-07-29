# InAppPurchasePriceScheduleCreateRequestIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | [optional] 
**attributes** | [**InAppPurchasePriceInlineCreateAttributes**](InAppPurchasePriceInlineCreateAttributes.md) |  | [optional] 
**relationships** | [**InAppPurchasePriceInlineCreateRelationships**](InAppPurchasePriceInlineCreateRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_price_schedule_create_request_included_inner import InAppPurchasePriceScheduleCreateRequestIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePriceScheduleCreateRequestIncludedInner from a JSON string
in_app_purchase_price_schedule_create_request_included_inner_instance = InAppPurchasePriceScheduleCreateRequestIncludedInner.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePriceScheduleCreateRequestIncludedInner.to_json())

# convert the object into a dict
in_app_purchase_price_schedule_create_request_included_inner_dict = in_app_purchase_price_schedule_create_request_included_inner_instance.to_dict()
# create an instance of InAppPurchasePriceScheduleCreateRequestIncludedInner from a dict
in_app_purchase_price_schedule_create_request_included_inner_from_dict = InAppPurchasePriceScheduleCreateRequestIncludedInner.from_dict(in_app_purchase_price_schedule_create_request_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


