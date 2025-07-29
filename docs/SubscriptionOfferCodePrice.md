# SubscriptionOfferCodePrice


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**relationships** | [**SubscriptionOfferCodePriceRelationships**](SubscriptionOfferCodePriceRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_price import SubscriptionOfferCodePrice

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodePrice from a JSON string
subscription_offer_code_price_instance = SubscriptionOfferCodePrice.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodePrice.to_json())

# convert the object into a dict
subscription_offer_code_price_dict = subscription_offer_code_price_instance.to_dict()
# create an instance of SubscriptionOfferCodePrice from a dict
subscription_offer_code_price_from_dict = SubscriptionOfferCodePrice.from_dict(subscription_offer_code_price_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


