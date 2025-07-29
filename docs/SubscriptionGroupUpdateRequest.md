# SubscriptionGroupUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionGroupUpdateRequestData**](SubscriptionGroupUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.subscription_group_update_request import SubscriptionGroupUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupUpdateRequest from a JSON string
subscription_group_update_request_instance = SubscriptionGroupUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupUpdateRequest.to_json())

# convert the object into a dict
subscription_group_update_request_dict = subscription_group_update_request_instance.to_dict()
# create an instance of SubscriptionGroupUpdateRequest from a dict
subscription_group_update_request_from_dict = SubscriptionGroupUpdateRequest.from_dict(subscription_group_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


