# SubscriptionOfferCodeCustomCodeCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionOfferCodeCustomCodeCreateRequestData**](SubscriptionOfferCodeCustomCodeCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.subscription_offer_code_custom_code_create_request import SubscriptionOfferCodeCustomCodeCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeCustomCodeCreateRequest from a JSON string
subscription_offer_code_custom_code_create_request_instance = SubscriptionOfferCodeCustomCodeCreateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeCustomCodeCreateRequest.to_json())

# convert the object into a dict
subscription_offer_code_custom_code_create_request_dict = subscription_offer_code_custom_code_create_request_instance.to_dict()
# create an instance of SubscriptionOfferCodeCustomCodeCreateRequest from a dict
subscription_offer_code_custom_code_create_request_from_dict = SubscriptionOfferCodeCustomCodeCreateRequest.from_dict(subscription_offer_code_custom_code_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


