# SubscriptionPromotionalOfferPricesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionPromotionalOfferPrice]**](SubscriptionPromotionalOfferPrice.md) |  | 
**included** | [**List[SubscriptionOfferCodePricesResponseIncludedInner]**](SubscriptionOfferCodePricesResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_promotional_offer_prices_response import SubscriptionPromotionalOfferPricesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotionalOfferPricesResponse from a JSON string
subscription_promotional_offer_prices_response_instance = SubscriptionPromotionalOfferPricesResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotionalOfferPricesResponse.to_json())

# convert the object into a dict
subscription_promotional_offer_prices_response_dict = subscription_promotional_offer_prices_response_instance.to_dict()
# create an instance of SubscriptionPromotionalOfferPricesResponse from a dict
subscription_promotional_offer_prices_response_from_dict = SubscriptionPromotionalOfferPricesResponse.from_dict(subscription_promotional_offer_prices_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


