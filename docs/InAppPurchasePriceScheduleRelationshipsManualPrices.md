# InAppPurchasePriceScheduleRelationshipsManualPrices


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[InAppPurchasePriceScheduleRelationshipsManualPricesDataInner]**](InAppPurchasePriceScheduleRelationshipsManualPricesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_price_schedule_relationships_manual_prices import InAppPurchasePriceScheduleRelationshipsManualPrices

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePriceScheduleRelationshipsManualPrices from a JSON string
in_app_purchase_price_schedule_relationships_manual_prices_instance = InAppPurchasePriceScheduleRelationshipsManualPrices.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePriceScheduleRelationshipsManualPrices.to_json())

# convert the object into a dict
in_app_purchase_price_schedule_relationships_manual_prices_dict = in_app_purchase_price_schedule_relationships_manual_prices_instance.to_dict()
# create an instance of InAppPurchasePriceScheduleRelationshipsManualPrices from a dict
in_app_purchase_price_schedule_relationships_manual_prices_from_dict = InAppPurchasePriceScheduleRelationshipsManualPrices.from_dict(in_app_purchase_price_schedule_relationships_manual_prices_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


