# InAppPurchaseV2Relationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**in_app_purchase_localizations** | [**InAppPurchaseV2RelationshipsInAppPurchaseLocalizations**](InAppPurchaseV2RelationshipsInAppPurchaseLocalizations.md) |  | [optional] 
**price_points** | [**InAppPurchaseV2RelationshipsPricePoints**](InAppPurchaseV2RelationshipsPricePoints.md) |  | [optional] 
**content** | [**InAppPurchaseV2RelationshipsContent**](InAppPurchaseV2RelationshipsContent.md) |  | [optional] 
**app_store_review_screenshot** | [**InAppPurchaseV2RelationshipsAppStoreReviewScreenshot**](InAppPurchaseV2RelationshipsAppStoreReviewScreenshot.md) |  | [optional] 
**promoted_purchase** | [**InAppPurchaseV2RelationshipsPromotedPurchase**](InAppPurchaseV2RelationshipsPromotedPurchase.md) |  | [optional] 
**iap_price_schedule** | [**InAppPurchaseV2RelationshipsIapPriceSchedule**](InAppPurchaseV2RelationshipsIapPriceSchedule.md) |  | [optional] 
**in_app_purchase_availability** | [**InAppPurchaseV2RelationshipsInAppPurchaseAvailability**](InAppPurchaseV2RelationshipsInAppPurchaseAvailability.md) |  | [optional] 
**images** | [**InAppPurchaseV2RelationshipsImages**](InAppPurchaseV2RelationshipsImages.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_v2_relationships import InAppPurchaseV2Relationships

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2Relationships from a JSON string
in_app_purchase_v2_relationships_instance = InAppPurchaseV2Relationships.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2Relationships.to_json())

# convert the object into a dict
in_app_purchase_v2_relationships_dict = in_app_purchase_v2_relationships_instance.to_dict()
# create an instance of InAppPurchaseV2Relationships from a dict
in_app_purchase_v2_relationships_from_dict = InAppPurchaseV2Relationships.from_dict(in_app_purchase_v2_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


