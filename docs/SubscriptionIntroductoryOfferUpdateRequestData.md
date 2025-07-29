# SubscriptionIntroductoryOfferUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionIntroductoryOfferUpdateRequestDataAttributes**](SubscriptionIntroductoryOfferUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_introductory_offer_update_request_data import SubscriptionIntroductoryOfferUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionIntroductoryOfferUpdateRequestData from a JSON string
subscription_introductory_offer_update_request_data_instance = SubscriptionIntroductoryOfferUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionIntroductoryOfferUpdateRequestData.to_json())

# convert the object into a dict
subscription_introductory_offer_update_request_data_dict = subscription_introductory_offer_update_request_data_instance.to_dict()
# create an instance of SubscriptionIntroductoryOfferUpdateRequestData from a dict
subscription_introductory_offer_update_request_data_from_dict = SubscriptionIntroductoryOfferUpdateRequestData.from_dict(subscription_introductory_offer_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


