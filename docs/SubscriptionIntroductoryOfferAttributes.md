# SubscriptionIntroductoryOfferAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**start_date** | **date** |  | [optional] 
**end_date** | **date** |  | [optional] 
**duration** | [**SubscriptionOfferDuration**](SubscriptionOfferDuration.md) |  | [optional] 
**offer_mode** | [**SubscriptionOfferMode**](SubscriptionOfferMode.md) |  | [optional] 
**number_of_periods** | **int** |  | [optional] 

## Example

```python
from openapi_client.models.subscription_introductory_offer_attributes import SubscriptionIntroductoryOfferAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionIntroductoryOfferAttributes from a JSON string
subscription_introductory_offer_attributes_instance = SubscriptionIntroductoryOfferAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionIntroductoryOfferAttributes.to_json())

# convert the object into a dict
subscription_introductory_offer_attributes_dict = subscription_introductory_offer_attributes_instance.to_dict()
# create an instance of SubscriptionIntroductoryOfferAttributes from a dict
subscription_introductory_offer_attributes_from_dict = SubscriptionIntroductoryOfferAttributes.from_dict(subscription_introductory_offer_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


