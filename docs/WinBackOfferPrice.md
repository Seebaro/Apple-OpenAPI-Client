# WinBackOfferPrice


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**relationships** | [**SubscriptionOfferCodePriceRelationships**](SubscriptionOfferCodePriceRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.win_back_offer_price import WinBackOfferPrice

# TODO update the JSON string below
json = "{}"
# create an instance of WinBackOfferPrice from a JSON string
win_back_offer_price_instance = WinBackOfferPrice.from_json(json)
# print the JSON string representation of the object
print(WinBackOfferPrice.to_json())

# convert the object into a dict
win_back_offer_price_dict = win_back_offer_price_instance.to_dict()
# create an instance of WinBackOfferPrice from a dict
win_back_offer_price_from_dict = WinBackOfferPrice.from_dict(win_back_offer_price_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


