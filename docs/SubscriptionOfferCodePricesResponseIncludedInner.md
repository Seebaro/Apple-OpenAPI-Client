# SubscriptionOfferCodePricesResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionPricePointAttributes**](SubscriptionPricePointAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 
**relationships** | [**InAppPurchasePricePointRelationships**](InAppPurchasePricePointRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_prices_response_included_inner import SubscriptionOfferCodePricesResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodePricesResponseIncludedInner from a JSON string
subscription_offer_code_prices_response_included_inner_instance = SubscriptionOfferCodePricesResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodePricesResponseIncludedInner.to_json())

# convert the object into a dict
subscription_offer_code_prices_response_included_inner_dict = subscription_offer_code_prices_response_included_inner_instance.to_dict()
# create an instance of SubscriptionOfferCodePricesResponseIncludedInner from a dict
subscription_offer_code_prices_response_included_inner_from_dict = SubscriptionOfferCodePricesResponseIncludedInner.from_dict(subscription_offer_code_prices_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


