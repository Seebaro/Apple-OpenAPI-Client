# SubscriptionPromotionalOfferInlineCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | [optional] 
**attributes** | [**SubscriptionPromotionalOfferInlineCreateAttributes**](SubscriptionPromotionalOfferInlineCreateAttributes.md) |  | 
**relationships** | [**SubscriptionPromotionalOfferInlineCreateRelationships**](SubscriptionPromotionalOfferInlineCreateRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_promotional_offer_inline_create import SubscriptionPromotionalOfferInlineCreate

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotionalOfferInlineCreate from a JSON string
subscription_promotional_offer_inline_create_instance = SubscriptionPromotionalOfferInlineCreate.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotionalOfferInlineCreate.to_json())

# convert the object into a dict
subscription_promotional_offer_inline_create_dict = subscription_promotional_offer_inline_create_instance.to_dict()
# create an instance of SubscriptionPromotionalOfferInlineCreate from a dict
subscription_promotional_offer_inline_create_from_dict = SubscriptionPromotionalOfferInlineCreate.from_dict(subscription_promotional_offer_inline_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


