# SubscriptionOfferCodeRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subscription** | [**PromotedPurchaseRelationshipsSubscription**](PromotedPurchaseRelationshipsSubscription.md) |  | [optional] 
**one_time_use_codes** | [**SubscriptionOfferCodeRelationshipsOneTimeUseCodes**](SubscriptionOfferCodeRelationshipsOneTimeUseCodes.md) |  | [optional] 
**custom_codes** | [**SubscriptionOfferCodeRelationshipsCustomCodes**](SubscriptionOfferCodeRelationshipsCustomCodes.md) |  | [optional] 
**prices** | [**SubscriptionOfferCodeRelationshipsPrices**](SubscriptionOfferCodeRelationshipsPrices.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_relationships import SubscriptionOfferCodeRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeRelationships from a JSON string
subscription_offer_code_relationships_instance = SubscriptionOfferCodeRelationships.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeRelationships.to_json())

# convert the object into a dict
subscription_offer_code_relationships_dict = subscription_offer_code_relationships_instance.to_dict()
# create an instance of SubscriptionOfferCodeRelationships from a dict
subscription_offer_code_relationships_from_dict = SubscriptionOfferCodeRelationships.from_dict(subscription_offer_code_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


