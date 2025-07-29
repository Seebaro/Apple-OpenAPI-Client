# SubscriptionIntroductoryOffer


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionIntroductoryOfferAttributes**](SubscriptionIntroductoryOfferAttributes.md) |  | [optional] 
**relationships** | [**SubscriptionIntroductoryOfferRelationships**](SubscriptionIntroductoryOfferRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_introductory_offer import SubscriptionIntroductoryOffer

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionIntroductoryOffer from a JSON string
subscription_introductory_offer_instance = SubscriptionIntroductoryOffer.from_json(json)
# print the JSON string representation of the object
print(SubscriptionIntroductoryOffer.to_json())

# convert the object into a dict
subscription_introductory_offer_dict = subscription_introductory_offer_instance.to_dict()
# create an instance of SubscriptionIntroductoryOffer from a dict
subscription_introductory_offer_from_dict = SubscriptionIntroductoryOffer.from_dict(subscription_introductory_offer_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


