# SubscriptionOfferCodeCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionOfferCodeCreateRequestData**](SubscriptionOfferCodeCreateRequestData.md) |  | 
**included** | [**List[SubscriptionOfferCodePriceInlineCreate]**](SubscriptionOfferCodePriceInlineCreate.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_create_request import SubscriptionOfferCodeCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeCreateRequest from a JSON string
subscription_offer_code_create_request_instance = SubscriptionOfferCodeCreateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeCreateRequest.to_json())

# convert the object into a dict
subscription_offer_code_create_request_dict = subscription_offer_code_create_request_instance.to_dict()
# create an instance of SubscriptionOfferCodeCreateRequest from a dict
subscription_offer_code_create_request_from_dict = SubscriptionOfferCodeCreateRequest.from_dict(subscription_offer_code_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


