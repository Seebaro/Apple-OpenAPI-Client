# SubscriptionOfferCodeUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionOfferCodeUpdateRequestData**](SubscriptionOfferCodeUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.subscription_offer_code_update_request import SubscriptionOfferCodeUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeUpdateRequest from a JSON string
subscription_offer_code_update_request_instance = SubscriptionOfferCodeUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeUpdateRequest.to_json())

# convert the object into a dict
subscription_offer_code_update_request_dict = subscription_offer_code_update_request_instance.to_dict()
# create an instance of SubscriptionOfferCodeUpdateRequest from a dict
subscription_offer_code_update_request_from_dict = SubscriptionOfferCodeUpdateRequest.from_dict(subscription_offer_code_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


