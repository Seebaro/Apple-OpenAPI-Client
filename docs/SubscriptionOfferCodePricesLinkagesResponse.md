# SubscriptionOfferCodePricesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionOfferCodeRelationshipsPricesDataInner]**](SubscriptionOfferCodeRelationshipsPricesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_prices_linkages_response import SubscriptionOfferCodePricesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodePricesLinkagesResponse from a JSON string
subscription_offer_code_prices_linkages_response_instance = SubscriptionOfferCodePricesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodePricesLinkagesResponse.to_json())

# convert the object into a dict
subscription_offer_code_prices_linkages_response_dict = subscription_offer_code_prices_linkages_response_instance.to_dict()
# create an instance of SubscriptionOfferCodePricesLinkagesResponse from a dict
subscription_offer_code_prices_linkages_response_from_dict = SubscriptionOfferCodePricesLinkagesResponse.from_dict(subscription_offer_code_prices_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


