# SubscriptionOfferCodePricesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionOfferCodePrice]**](SubscriptionOfferCodePrice.md) |  | 
**included** | [**List[SubscriptionOfferCodePricesResponseIncludedInner]**](SubscriptionOfferCodePricesResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_prices_response import SubscriptionOfferCodePricesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodePricesResponse from a JSON string
subscription_offer_code_prices_response_instance = SubscriptionOfferCodePricesResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodePricesResponse.to_json())

# convert the object into a dict
subscription_offer_code_prices_response_dict = subscription_offer_code_prices_response_instance.to_dict()
# create an instance of SubscriptionOfferCodePricesResponse from a dict
subscription_offer_code_prices_response_from_dict = SubscriptionOfferCodePricesResponse.from_dict(subscription_offer_code_prices_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


