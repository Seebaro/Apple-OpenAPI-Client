# InAppPurchasePriceScheduleCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**in_app_purchase** | [**InAppPurchaseAppStoreReviewScreenshotCreateRequestDataRelationshipsInAppPurchaseV2**](InAppPurchaseAppStoreReviewScreenshotCreateRequestDataRelationshipsInAppPurchaseV2.md) |  | 
**base_territory** | [**AppPriceScheduleCreateRequestDataRelationshipsBaseTerritory**](AppPriceScheduleCreateRequestDataRelationshipsBaseTerritory.md) |  | 
**manual_prices** | [**InAppPurchasePriceScheduleCreateRequestDataRelationshipsManualPrices**](InAppPurchasePriceScheduleCreateRequestDataRelationshipsManualPrices.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_price_schedule_create_request_data_relationships import InAppPurchasePriceScheduleCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePriceScheduleCreateRequestDataRelationships from a JSON string
in_app_purchase_price_schedule_create_request_data_relationships_instance = InAppPurchasePriceScheduleCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePriceScheduleCreateRequestDataRelationships.to_json())

# convert the object into a dict
in_app_purchase_price_schedule_create_request_data_relationships_dict = in_app_purchase_price_schedule_create_request_data_relationships_instance.to_dict()
# create an instance of InAppPurchasePriceScheduleCreateRequestDataRelationships from a dict
in_app_purchase_price_schedule_create_request_data_relationships_from_dict = InAppPurchasePriceScheduleCreateRequestDataRelationships.from_dict(in_app_purchase_price_schedule_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


