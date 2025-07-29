# WinBackOfferCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**WinBackOfferCreateRequestData**](WinBackOfferCreateRequestData.md) |  | 
**included** | [**List[WinBackOfferPriceInlineCreate]**](WinBackOfferPriceInlineCreate.md) |  | [optional] 

## Example

```python
from openapi_client.models.win_back_offer_create_request import WinBackOfferCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WinBackOfferCreateRequest from a JSON string
win_back_offer_create_request_instance = WinBackOfferCreateRequest.from_json(json)
# print the JSON string representation of the object
print(WinBackOfferCreateRequest.to_json())

# convert the object into a dict
win_back_offer_create_request_dict = win_back_offer_create_request_instance.to_dict()
# create an instance of WinBackOfferCreateRequest from a dict
win_back_offer_create_request_from_dict = WinBackOfferCreateRequest.from_dict(win_back_offer_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


