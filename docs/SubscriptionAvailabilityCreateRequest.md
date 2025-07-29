# SubscriptionAvailabilityCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionAvailabilityCreateRequestData**](SubscriptionAvailabilityCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.subscription_availability_create_request import SubscriptionAvailabilityCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionAvailabilityCreateRequest from a JSON string
subscription_availability_create_request_instance = SubscriptionAvailabilityCreateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionAvailabilityCreateRequest.to_json())

# convert the object into a dict
subscription_availability_create_request_dict = subscription_availability_create_request_instance.to_dict()
# create an instance of SubscriptionAvailabilityCreateRequest from a dict
subscription_availability_create_request_from_dict = SubscriptionAvailabilityCreateRequest.from_dict(subscription_availability_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


