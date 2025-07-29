# SubscriptionLocalizationUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionLocalizationUpdateRequestData**](SubscriptionLocalizationUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.subscription_localization_update_request import SubscriptionLocalizationUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionLocalizationUpdateRequest from a JSON string
subscription_localization_update_request_instance = SubscriptionLocalizationUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionLocalizationUpdateRequest.to_json())

# convert the object into a dict
subscription_localization_update_request_dict = subscription_localization_update_request_instance.to_dict()
# create an instance of SubscriptionLocalizationUpdateRequest from a dict
subscription_localization_update_request_from_dict = SubscriptionLocalizationUpdateRequest.from_dict(subscription_localization_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


