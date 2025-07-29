# InAppPurchasePriceScheduleRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**base_territory** | [**AppPriceScheduleRelationshipsBaseTerritory**](AppPriceScheduleRelationshipsBaseTerritory.md) |  | [optional] 
**manual_prices** | [**InAppPurchasePriceScheduleRelationshipsManualPrices**](InAppPurchasePriceScheduleRelationshipsManualPrices.md) |  | [optional] 
**automatic_prices** | [**InAppPurchasePriceScheduleRelationshipsManualPrices**](InAppPurchasePriceScheduleRelationshipsManualPrices.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_price_schedule_relationships import InAppPurchasePriceScheduleRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePriceScheduleRelationships from a JSON string
in_app_purchase_price_schedule_relationships_instance = InAppPurchasePriceScheduleRelationships.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePriceScheduleRelationships.to_json())

# convert the object into a dict
in_app_purchase_price_schedule_relationships_dict = in_app_purchase_price_schedule_relationships_instance.to_dict()
# create an instance of InAppPurchasePriceScheduleRelationships from a dict
in_app_purchase_price_schedule_relationships_from_dict = InAppPurchasePriceScheduleRelationships.from_dict(in_app_purchase_price_schedule_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


