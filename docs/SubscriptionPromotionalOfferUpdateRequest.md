# SubscriptionPromotionalOfferUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionPromotionalOfferUpdateRequestData**](SubscriptionPromotionalOfferUpdateRequestData.md) |  | 
**included** | [**List[SubscriptionPromotionalOfferPriceInlineCreate]**](SubscriptionPromotionalOfferPriceInlineCreate.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_promotional_offer_update_request import SubscriptionPromotionalOfferUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotionalOfferUpdateRequest from a JSON string
subscription_promotional_offer_update_request_instance = SubscriptionPromotionalOfferUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotionalOfferUpdateRequest.to_json())

# convert the object into a dict
subscription_promotional_offer_update_request_dict = subscription_promotional_offer_update_request_instance.to_dict()
# create an instance of SubscriptionPromotionalOfferUpdateRequest from a dict
subscription_promotional_offer_update_request_from_dict = SubscriptionPromotionalOfferUpdateRequest.from_dict(subscription_promotional_offer_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


