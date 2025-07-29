# SubscriptionIntroductoryOfferCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**SubscriptionIntroductoryOfferInlineCreateAttributes**](SubscriptionIntroductoryOfferInlineCreateAttributes.md) |  | 
**relationships** | [**SubscriptionIntroductoryOfferCreateRequestDataRelationships**](SubscriptionIntroductoryOfferCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.subscription_introductory_offer_create_request_data import SubscriptionIntroductoryOfferCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionIntroductoryOfferCreateRequestData from a JSON string
subscription_introductory_offer_create_request_data_instance = SubscriptionIntroductoryOfferCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionIntroductoryOfferCreateRequestData.to_json())

# convert the object into a dict
subscription_introductory_offer_create_request_data_dict = subscription_introductory_offer_create_request_data_instance.to_dict()
# create an instance of SubscriptionIntroductoryOfferCreateRequestData from a dict
subscription_introductory_offer_create_request_data_from_dict = SubscriptionIntroductoryOfferCreateRequestData.from_dict(subscription_introductory_offer_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


