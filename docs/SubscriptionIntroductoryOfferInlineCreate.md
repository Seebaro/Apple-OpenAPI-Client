# SubscriptionIntroductoryOfferInlineCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | [optional] 
**attributes** | [**SubscriptionIntroductoryOfferInlineCreateAttributes**](SubscriptionIntroductoryOfferInlineCreateAttributes.md) |  | 
**relationships** | [**SubscriptionIntroductoryOfferRelationships**](SubscriptionIntroductoryOfferRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_introductory_offer_inline_create import SubscriptionIntroductoryOfferInlineCreate

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionIntroductoryOfferInlineCreate from a JSON string
subscription_introductory_offer_inline_create_instance = SubscriptionIntroductoryOfferInlineCreate.from_json(json)
# print the JSON string representation of the object
print(SubscriptionIntroductoryOfferInlineCreate.to_json())

# convert the object into a dict
subscription_introductory_offer_inline_create_dict = subscription_introductory_offer_inline_create_instance.to_dict()
# create an instance of SubscriptionIntroductoryOfferInlineCreate from a dict
subscription_introductory_offer_inline_create_from_dict = SubscriptionIntroductoryOfferInlineCreate.from_dict(subscription_introductory_offer_inline_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


