# SubscriptionPromotionalOfferPricesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionPromotionalOfferRelationshipsPricesDataInner]**](SubscriptionPromotionalOfferRelationshipsPricesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_promotional_offer_prices_linkages_response import SubscriptionPromotionalOfferPricesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotionalOfferPricesLinkagesResponse from a JSON string
subscription_promotional_offer_prices_linkages_response_instance = SubscriptionPromotionalOfferPricesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotionalOfferPricesLinkagesResponse.to_json())

# convert the object into a dict
subscription_promotional_offer_prices_linkages_response_dict = subscription_promotional_offer_prices_linkages_response_instance.to_dict()
# create an instance of SubscriptionPromotionalOfferPricesLinkagesResponse from a dict
subscription_promotional_offer_prices_linkages_response_from_dict = SubscriptionPromotionalOfferPricesLinkagesResponse.from_dict(subscription_promotional_offer_prices_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


