# SubscriptionOfferCodePriceInlineCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | [optional] 
**relationships** | [**SubscriptionOfferCodePriceRelationships**](SubscriptionOfferCodePriceRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_price_inline_create import SubscriptionOfferCodePriceInlineCreate

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodePriceInlineCreate from a JSON string
subscription_offer_code_price_inline_create_instance = SubscriptionOfferCodePriceInlineCreate.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodePriceInlineCreate.to_json())

# convert the object into a dict
subscription_offer_code_price_inline_create_dict = subscription_offer_code_price_inline_create_instance.to_dict()
# create an instance of SubscriptionOfferCodePriceInlineCreate from a dict
subscription_offer_code_price_inline_create_from_dict = SubscriptionOfferCodePriceInlineCreate.from_dict(subscription_offer_code_price_inline_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


