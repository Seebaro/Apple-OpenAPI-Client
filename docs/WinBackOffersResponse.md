# WinBackOffersResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[WinBackOffer]**](WinBackOffer.md) |  | 
**included** | [**List[WinBackOfferPrice]**](WinBackOfferPrice.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.win_back_offers_response import WinBackOffersResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WinBackOffersResponse from a JSON string
win_back_offers_response_instance = WinBackOffersResponse.from_json(json)
# print the JSON string representation of the object
print(WinBackOffersResponse.to_json())

# convert the object into a dict
win_back_offers_response_dict = win_back_offers_response_instance.to_dict()
# create an instance of WinBackOffersResponse from a dict
win_back_offers_response_from_dict = WinBackOffersResponse.from_dict(win_back_offers_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


