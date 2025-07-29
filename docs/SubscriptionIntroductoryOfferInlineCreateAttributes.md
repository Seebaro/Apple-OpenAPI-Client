# SubscriptionIntroductoryOfferInlineCreateAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**start_date** | **date** |  | [optional] 
**end_date** | **date** |  | [optional] 
**duration** | [**SubscriptionOfferDuration**](SubscriptionOfferDuration.md) |  | 
**offer_mode** | [**SubscriptionOfferMode**](SubscriptionOfferMode.md) |  | 
**number_of_periods** | **int** |  | 

## Example

```python
from openapi_client.models.subscription_introductory_offer_inline_create_attributes import SubscriptionIntroductoryOfferInlineCreateAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionIntroductoryOfferInlineCreateAttributes from a JSON string
subscription_introductory_offer_inline_create_attributes_instance = SubscriptionIntroductoryOfferInlineCreateAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionIntroductoryOfferInlineCreateAttributes.to_json())

# convert the object into a dict
subscription_introductory_offer_inline_create_attributes_dict = subscription_introductory_offer_inline_create_attributes_instance.to_dict()
# create an instance of SubscriptionIntroductoryOfferInlineCreateAttributes from a dict
subscription_introductory_offer_inline_create_attributes_from_dict = SubscriptionIntroductoryOfferInlineCreateAttributes.from_dict(subscription_introductory_offer_inline_create_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


