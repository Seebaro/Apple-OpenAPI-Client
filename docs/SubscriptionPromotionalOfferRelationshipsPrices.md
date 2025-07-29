# SubscriptionPromotionalOfferRelationshipsPrices


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[SubscriptionPromotionalOfferRelationshipsPricesDataInner]**](SubscriptionPromotionalOfferRelationshipsPricesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_promotional_offer_relationships_prices import SubscriptionPromotionalOfferRelationshipsPrices

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotionalOfferRelationshipsPrices from a JSON string
subscription_promotional_offer_relationships_prices_instance = SubscriptionPromotionalOfferRelationshipsPrices.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotionalOfferRelationshipsPrices.to_json())

# convert the object into a dict
subscription_promotional_offer_relationships_prices_dict = subscription_promotional_offer_relationships_prices_instance.to_dict()
# create an instance of SubscriptionPromotionalOfferRelationshipsPrices from a dict
subscription_promotional_offer_relationships_prices_from_dict = SubscriptionPromotionalOfferRelationshipsPrices.from_dict(subscription_promotional_offer_relationships_prices_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


