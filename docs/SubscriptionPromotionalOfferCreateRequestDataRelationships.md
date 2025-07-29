# SubscriptionPromotionalOfferCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subscription** | [**SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationshipsSubscription**](SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationshipsSubscription.md) |  | 
**prices** | [**SubscriptionPromotionalOfferCreateRequestDataRelationshipsPrices**](SubscriptionPromotionalOfferCreateRequestDataRelationshipsPrices.md) |  | 

## Example

```python
from openapi_client.models.subscription_promotional_offer_create_request_data_relationships import SubscriptionPromotionalOfferCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotionalOfferCreateRequestDataRelationships from a JSON string
subscription_promotional_offer_create_request_data_relationships_instance = SubscriptionPromotionalOfferCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotionalOfferCreateRequestDataRelationships.to_json())

# convert the object into a dict
subscription_promotional_offer_create_request_data_relationships_dict = subscription_promotional_offer_create_request_data_relationships_instance.to_dict()
# create an instance of SubscriptionPromotionalOfferCreateRequestDataRelationships from a dict
subscription_promotional_offer_create_request_data_relationships_from_dict = SubscriptionPromotionalOfferCreateRequestDataRelationships.from_dict(subscription_promotional_offer_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


