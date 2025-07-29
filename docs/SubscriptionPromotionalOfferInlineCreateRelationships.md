# SubscriptionPromotionalOfferInlineCreateRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subscription** | [**PromotedPurchaseRelationshipsSubscription**](PromotedPurchaseRelationshipsSubscription.md) |  | [optional] 
**prices** | [**SubscriptionPromotionalOfferInlineCreateRelationshipsPrices**](SubscriptionPromotionalOfferInlineCreateRelationshipsPrices.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_promotional_offer_inline_create_relationships import SubscriptionPromotionalOfferInlineCreateRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotionalOfferInlineCreateRelationships from a JSON string
subscription_promotional_offer_inline_create_relationships_instance = SubscriptionPromotionalOfferInlineCreateRelationships.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotionalOfferInlineCreateRelationships.to_json())

# convert the object into a dict
subscription_promotional_offer_inline_create_relationships_dict = subscription_promotional_offer_inline_create_relationships_instance.to_dict()
# create an instance of SubscriptionPromotionalOfferInlineCreateRelationships from a dict
subscription_promotional_offer_inline_create_relationships_from_dict = SubscriptionPromotionalOfferInlineCreateRelationships.from_dict(subscription_promotional_offer_inline_create_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


