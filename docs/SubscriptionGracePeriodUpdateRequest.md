# SubscriptionGracePeriodUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionGracePeriodUpdateRequestData**](SubscriptionGracePeriodUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.subscription_grace_period_update_request import SubscriptionGracePeriodUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGracePeriodUpdateRequest from a JSON string
subscription_grace_period_update_request_instance = SubscriptionGracePeriodUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGracePeriodUpdateRequest.to_json())

# convert the object into a dict
subscription_grace_period_update_request_dict = subscription_grace_period_update_request_instance.to_dict()
# create an instance of SubscriptionGracePeriodUpdateRequest from a dict
subscription_grace_period_update_request_from_dict = SubscriptionGracePeriodUpdateRequest.from_dict(subscription_grace_period_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


