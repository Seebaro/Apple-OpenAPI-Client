# SubscriptionGroupLocalizationUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionGroupLocalizationUpdateRequestData**](SubscriptionGroupLocalizationUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.subscription_group_localization_update_request import SubscriptionGroupLocalizationUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupLocalizationUpdateRequest from a JSON string
subscription_group_localization_update_request_instance = SubscriptionGroupLocalizationUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupLocalizationUpdateRequest.to_json())

# convert the object into a dict
subscription_group_localization_update_request_dict = subscription_group_localization_update_request_instance.to_dict()
# create an instance of SubscriptionGroupLocalizationUpdateRequest from a dict
subscription_group_localization_update_request_from_dict = SubscriptionGroupLocalizationUpdateRequest.from_dict(subscription_group_localization_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


