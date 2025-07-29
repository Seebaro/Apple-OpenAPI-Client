# SubscriptionPriceInlineCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | [optional] 
**attributes** | [**SubscriptionPriceInlineCreateAttributes**](SubscriptionPriceInlineCreateAttributes.md) |  | [optional] 
**relationships** | [**SubscriptionIntroductoryOfferRelationships**](SubscriptionIntroductoryOfferRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_price_inline_create import SubscriptionPriceInlineCreate

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPriceInlineCreate from a JSON string
subscription_price_inline_create_instance = SubscriptionPriceInlineCreate.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPriceInlineCreate.to_json())

# convert the object into a dict
subscription_price_inline_create_dict = subscription_price_inline_create_instance.to_dict()
# create an instance of SubscriptionPriceInlineCreate from a dict
subscription_price_inline_create_from_dict = SubscriptionPriceInlineCreate.from_dict(subscription_price_inline_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


