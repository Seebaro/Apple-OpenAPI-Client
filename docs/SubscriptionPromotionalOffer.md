# SubscriptionPromotionalOffer


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionPromotionalOfferAttributes**](SubscriptionPromotionalOfferAttributes.md) |  | [optional] 
**relationships** | [**SubscriptionPromotionalOfferRelationships**](SubscriptionPromotionalOfferRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_promotional_offer import SubscriptionPromotionalOffer

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotionalOffer from a JSON string
subscription_promotional_offer_instance = SubscriptionPromotionalOffer.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotionalOffer.to_json())

# convert the object into a dict
subscription_promotional_offer_dict = subscription_promotional_offer_instance.to_dict()
# create an instance of SubscriptionPromotionalOffer from a dict
subscription_promotional_offer_from_dict = SubscriptionPromotionalOffer.from_dict(subscription_promotional_offer_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


