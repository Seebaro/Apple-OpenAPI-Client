# SubscriptionCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionCreateRequestData**](SubscriptionCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.subscription_create_request import SubscriptionCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionCreateRequest from a JSON string
subscription_create_request_instance = SubscriptionCreateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionCreateRequest.to_json())

# convert the object into a dict
subscription_create_request_dict = subscription_create_request_instance.to_dict()
# create an instance of SubscriptionCreateRequest from a dict
subscription_create_request_from_dict = SubscriptionCreateRequest.from_dict(subscription_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


