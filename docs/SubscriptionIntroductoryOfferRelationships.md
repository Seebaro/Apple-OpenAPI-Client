# SubscriptionIntroductoryOfferRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subscription** | [**PromotedPurchaseRelationshipsSubscription**](PromotedPurchaseRelationshipsSubscription.md) |  | [optional] 
**territory** | [**AppPricePointV3RelationshipsTerritory**](AppPricePointV3RelationshipsTerritory.md) |  | [optional] 
**subscription_price_point** | [**SubscriptionIntroductoryOfferRelationshipsSubscriptionPricePoint**](SubscriptionIntroductoryOfferRelationshipsSubscriptionPricePoint.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_introductory_offer_relationships import SubscriptionIntroductoryOfferRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionIntroductoryOfferRelationships from a JSON string
subscription_introductory_offer_relationships_instance = SubscriptionIntroductoryOfferRelationships.from_json(json)
# print the JSON string representation of the object
print(SubscriptionIntroductoryOfferRelationships.to_json())

# convert the object into a dict
subscription_introductory_offer_relationships_dict = subscription_introductory_offer_relationships_instance.to_dict()
# create an instance of SubscriptionIntroductoryOfferRelationships from a dict
subscription_introductory_offer_relationships_from_dict = SubscriptionIntroductoryOfferRelationships.from_dict(subscription_introductory_offer_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


