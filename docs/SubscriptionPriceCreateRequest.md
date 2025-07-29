# SubscriptionPriceCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionPriceCreateRequestData**](SubscriptionPriceCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.subscription_price_create_request import SubscriptionPriceCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPriceCreateRequest from a JSON string
subscription_price_create_request_instance = SubscriptionPriceCreateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPriceCreateRequest.to_json())

# convert the object into a dict
subscription_price_create_request_dict = subscription_price_create_request_instance.to_dict()
# create an instance of SubscriptionPriceCreateRequest from a dict
subscription_price_create_request_from_dict = SubscriptionPriceCreateRequest.from_dict(subscription_price_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


