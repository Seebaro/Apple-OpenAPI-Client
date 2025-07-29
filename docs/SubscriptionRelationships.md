# SubscriptionRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subscription_localizations** | [**SubscriptionRelationshipsSubscriptionLocalizations**](SubscriptionRelationshipsSubscriptionLocalizations.md) |  | [optional] 
**app_store_review_screenshot** | [**SubscriptionRelationshipsAppStoreReviewScreenshot**](SubscriptionRelationshipsAppStoreReviewScreenshot.md) |  | [optional] 
**group** | [**SubscriptionGroupLocalizationRelationshipsSubscriptionGroup**](SubscriptionGroupLocalizationRelationshipsSubscriptionGroup.md) |  | [optional] 
**introductory_offers** | [**SubscriptionRelationshipsIntroductoryOffers**](SubscriptionRelationshipsIntroductoryOffers.md) |  | [optional] 
**promotional_offers** | [**SubscriptionRelationshipsPromotionalOffers**](SubscriptionRelationshipsPromotionalOffers.md) |  | [optional] 
**offer_codes** | [**SubscriptionRelationshipsOfferCodes**](SubscriptionRelationshipsOfferCodes.md) |  | [optional] 
**prices** | [**SubscriptionRelationshipsPrices**](SubscriptionRelationshipsPrices.md) |  | [optional] 
**price_points** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**promoted_purchase** | [**InAppPurchaseV2RelationshipsPromotedPurchase**](InAppPurchaseV2RelationshipsPromotedPurchase.md) |  | [optional] 
**subscription_availability** | [**SubscriptionRelationshipsSubscriptionAvailability**](SubscriptionRelationshipsSubscriptionAvailability.md) |  | [optional] 
**win_back_offers** | [**SubscriptionRelationshipsWinBackOffers**](SubscriptionRelationshipsWinBackOffers.md) |  | [optional] 
**images** | [**SubscriptionRelationshipsImages**](SubscriptionRelationshipsImages.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_relationships import SubscriptionRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionRelationships from a JSON string
subscription_relationships_instance = SubscriptionRelationships.from_json(json)
# print the JSON string representation of the object
print(SubscriptionRelationships.to_json())

# convert the object into a dict
subscription_relationships_dict = subscription_relationships_instance.to_dict()
# create an instance of SubscriptionRelationships from a dict
subscription_relationships_from_dict = SubscriptionRelationships.from_dict(subscription_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


