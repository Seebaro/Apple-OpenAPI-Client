# WinBackOfferPricesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[WinBackOfferRelationshipsPricesDataInner]**](WinBackOfferRelationshipsPricesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.win_back_offer_prices_linkages_response import WinBackOfferPricesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WinBackOfferPricesLinkagesResponse from a JSON string
win_back_offer_prices_linkages_response_instance = WinBackOfferPricesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(WinBackOfferPricesLinkagesResponse.to_json())

# convert the object into a dict
win_back_offer_prices_linkages_response_dict = win_back_offer_prices_linkages_response_instance.to_dict()
# create an instance of WinBackOfferPricesLinkagesResponse from a dict
win_back_offer_prices_linkages_response_from_dict = WinBackOfferPricesLinkagesResponse.from_dict(win_back_offer_prices_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


