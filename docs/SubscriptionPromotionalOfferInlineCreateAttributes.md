# SubscriptionPromotionalOfferInlineCreateAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**duration** | [**SubscriptionOfferDuration**](SubscriptionOfferDuration.md) |  | 
**name** | **str** |  | 
**number_of_periods** | **int** |  | 
**offer_code** | **str** |  | 
**offer_mode** | [**SubscriptionOfferMode**](SubscriptionOfferMode.md) |  | 

## Example

```python
from openapi_client.models.subscription_promotional_offer_inline_create_attributes import SubscriptionPromotionalOfferInlineCreateAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotionalOfferInlineCreateAttributes from a JSON string
subscription_promotional_offer_inline_create_attributes_instance = SubscriptionPromotionalOfferInlineCreateAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotionalOfferInlineCreateAttributes.to_json())

# convert the object into a dict
subscription_promotional_offer_inline_create_attributes_dict = subscription_promotional_offer_inline_create_attributes_instance.to_dict()
# create an instance of SubscriptionPromotionalOfferInlineCreateAttributes from a dict
subscription_promotional_offer_inline_create_attributes_from_dict = SubscriptionPromotionalOfferInlineCreateAttributes.from_dict(subscription_promotional_offer_inline_create_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


