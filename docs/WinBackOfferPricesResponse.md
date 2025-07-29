# WinBackOfferPricesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[WinBackOfferPrice]**](WinBackOfferPrice.md) |  | 
**included** | [**List[SubscriptionOfferCodePricesResponseIncludedInner]**](SubscriptionOfferCodePricesResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.win_back_offer_prices_response import WinBackOfferPricesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WinBackOfferPricesResponse from a JSON string
win_back_offer_prices_response_instance = WinBackOfferPricesResponse.from_json(json)
# print the JSON string representation of the object
print(WinBackOfferPricesResponse.to_json())

# convert the object into a dict
win_back_offer_prices_response_dict = win_back_offer_prices_response_instance.to_dict()
# create an instance of WinBackOfferPricesResponse from a dict
win_back_offer_prices_response_from_dict = WinBackOfferPricesResponse.from_dict(win_back_offer_prices_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


