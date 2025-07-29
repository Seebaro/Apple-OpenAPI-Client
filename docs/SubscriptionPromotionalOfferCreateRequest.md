# SubscriptionPromotionalOfferCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionPromotionalOfferCreateRequestData**](SubscriptionPromotionalOfferCreateRequestData.md) |  | 
**included** | [**List[SubscriptionPromotionalOfferPriceInlineCreate]**](SubscriptionPromotionalOfferPriceInlineCreate.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_promotional_offer_create_request import SubscriptionPromotionalOfferCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotionalOfferCreateRequest from a JSON string
subscription_promotional_offer_create_request_instance = SubscriptionPromotionalOfferCreateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotionalOfferCreateRequest.to_json())

# convert the object into a dict
subscription_promotional_offer_create_request_dict = subscription_promotional_offer_create_request_instance.to_dict()
# create an instance of SubscriptionPromotionalOfferCreateRequest from a dict
subscription_promotional_offer_create_request_from_dict = SubscriptionPromotionalOfferCreateRequest.from_dict(subscription_promotional_offer_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


