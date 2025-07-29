# WinBackOfferResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**WinBackOffer**](WinBackOffer.md) |  | 
**included** | [**List[WinBackOfferPrice]**](WinBackOfferPrice.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.win_back_offer_response import WinBackOfferResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WinBackOfferResponse from a JSON string
win_back_offer_response_instance = WinBackOfferResponse.from_json(json)
# print the JSON string representation of the object
print(WinBackOfferResponse.to_json())

# convert the object into a dict
win_back_offer_response_dict = win_back_offer_response_instance.to_dict()
# create an instance of WinBackOfferResponse from a dict
win_back_offer_response_from_dict = WinBackOfferResponse.from_dict(win_back_offer_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


