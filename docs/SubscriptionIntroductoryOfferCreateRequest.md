# SubscriptionIntroductoryOfferCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionIntroductoryOfferCreateRequestData**](SubscriptionIntroductoryOfferCreateRequestData.md) |  | 
**included** | [**List[SubscriptionPricePointInlineCreate]**](SubscriptionPricePointInlineCreate.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_introductory_offer_create_request import SubscriptionIntroductoryOfferCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionIntroductoryOfferCreateRequest from a JSON string
subscription_introductory_offer_create_request_instance = SubscriptionIntroductoryOfferCreateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionIntroductoryOfferCreateRequest.to_json())

# convert the object into a dict
subscription_introductory_offer_create_request_dict = subscription_introductory_offer_create_request_instance.to_dict()
# create an instance of SubscriptionIntroductoryOfferCreateRequest from a dict
subscription_introductory_offer_create_request_from_dict = SubscriptionIntroductoryOfferCreateRequest.from_dict(subscription_introductory_offer_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


