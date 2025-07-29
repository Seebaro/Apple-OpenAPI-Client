# SubscriptionPromotionalOfferResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionPromotionalOffer**](SubscriptionPromotionalOffer.md) |  | 
**included** | [**List[SubscriptionPromotionalOffersResponseIncludedInner]**](SubscriptionPromotionalOffersResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_promotional_offer_response import SubscriptionPromotionalOfferResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotionalOfferResponse from a JSON string
subscription_promotional_offer_response_instance = SubscriptionPromotionalOfferResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotionalOfferResponse.to_json())

# convert the object into a dict
subscription_promotional_offer_response_dict = subscription_promotional_offer_response_instance.to_dict()
# create an instance of SubscriptionPromotionalOfferResponse from a dict
subscription_promotional_offer_response_from_dict = SubscriptionPromotionalOfferResponse.from_dict(subscription_promotional_offer_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


