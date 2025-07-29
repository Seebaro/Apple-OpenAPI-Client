# SubscriptionIntroductoryOfferResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionIntroductoryOffer**](SubscriptionIntroductoryOffer.md) |  | 
**included** | [**List[SubscriptionIntroductoryOffersResponseIncludedInner]**](SubscriptionIntroductoryOffersResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_introductory_offer_response import SubscriptionIntroductoryOfferResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionIntroductoryOfferResponse from a JSON string
subscription_introductory_offer_response_instance = SubscriptionIntroductoryOfferResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionIntroductoryOfferResponse.to_json())

# convert the object into a dict
subscription_introductory_offer_response_dict = subscription_introductory_offer_response_instance.to_dict()
# create an instance of SubscriptionIntroductoryOfferResponse from a dict
subscription_introductory_offer_response_from_dict = SubscriptionIntroductoryOfferResponse.from_dict(subscription_introductory_offer_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


