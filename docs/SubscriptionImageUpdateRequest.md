# SubscriptionImageUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionImageUpdateRequestData**](SubscriptionImageUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.subscription_image_update_request import SubscriptionImageUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionImageUpdateRequest from a JSON string
subscription_image_update_request_instance = SubscriptionImageUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionImageUpdateRequest.to_json())

# convert the object into a dict
subscription_image_update_request_dict = subscription_image_update_request_instance.to_dict()
# create an instance of SubscriptionImageUpdateRequest from a dict
subscription_image_update_request_from_dict = SubscriptionImageUpdateRequest.from_dict(subscription_image_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


