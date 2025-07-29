# SubscriptionOfferCodePriceRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**territory** | [**AppPricePointV3RelationshipsTerritory**](AppPricePointV3RelationshipsTerritory.md) |  | [optional] 
**subscription_price_point** | [**SubscriptionIntroductoryOfferRelationshipsSubscriptionPricePoint**](SubscriptionIntroductoryOfferRelationshipsSubscriptionPricePoint.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_price_relationships import SubscriptionOfferCodePriceRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodePriceRelationships from a JSON string
subscription_offer_code_price_relationships_instance = SubscriptionOfferCodePriceRelationships.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodePriceRelationships.to_json())

# convert the object into a dict
subscription_offer_code_price_relationships_dict = subscription_offer_code_price_relationships_instance.to_dict()
# create an instance of SubscriptionOfferCodePriceRelationships from a dict
subscription_offer_code_price_relationships_from_dict = SubscriptionOfferCodePriceRelationships.from_dict(subscription_offer_code_price_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


