# SubscriptionOfferCodeRelationshipsPrices


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[SubscriptionOfferCodeRelationshipsPricesDataInner]**](SubscriptionOfferCodeRelationshipsPricesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_relationships_prices import SubscriptionOfferCodeRelationshipsPrices

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeRelationshipsPrices from a JSON string
subscription_offer_code_relationships_prices_instance = SubscriptionOfferCodeRelationshipsPrices.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeRelationshipsPrices.to_json())

# convert the object into a dict
subscription_offer_code_relationships_prices_dict = subscription_offer_code_relationships_prices_instance.to_dict()
# create an instance of SubscriptionOfferCodeRelationshipsPrices from a dict
subscription_offer_code_relationships_prices_from_dict = SubscriptionOfferCodeRelationshipsPrices.from_dict(subscription_offer_code_relationships_prices_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


