# SubscriptionIntroductoryOfferUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionIntroductoryOfferUpdateRequestData**](SubscriptionIntroductoryOfferUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.subscription_introductory_offer_update_request import SubscriptionIntroductoryOfferUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionIntroductoryOfferUpdateRequest from a JSON string
subscription_introductory_offer_update_request_instance = SubscriptionIntroductoryOfferUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionIntroductoryOfferUpdateRequest.to_json())

# convert the object into a dict
subscription_introductory_offer_update_request_dict = subscription_introductory_offer_update_request_instance.to_dict()
# create an instance of SubscriptionIntroductoryOfferUpdateRequest from a dict
subscription_introductory_offer_update_request_from_dict = SubscriptionIntroductoryOfferUpdateRequest.from_dict(subscription_introductory_offer_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


