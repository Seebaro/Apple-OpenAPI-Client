# SubscriptionPromotionalOfferPrice


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**relationships** | [**SubscriptionOfferCodePriceRelationships**](SubscriptionOfferCodePriceRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_promotional_offer_price import SubscriptionPromotionalOfferPrice

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotionalOfferPrice from a JSON string
subscription_promotional_offer_price_instance = SubscriptionPromotionalOfferPrice.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotionalOfferPrice.to_json())

# convert the object into a dict
subscription_promotional_offer_price_dict = subscription_promotional_offer_price_instance.to_dict()
# create an instance of SubscriptionPromotionalOfferPrice from a dict
subscription_promotional_offer_price_from_dict = SubscriptionPromotionalOfferPrice.from_dict(subscription_promotional_offer_price_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


