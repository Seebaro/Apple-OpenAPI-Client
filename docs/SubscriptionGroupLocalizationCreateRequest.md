# SubscriptionGroupLocalizationCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionGroupLocalizationCreateRequestData**](SubscriptionGroupLocalizationCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.subscription_group_localization_create_request import SubscriptionGroupLocalizationCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupLocalizationCreateRequest from a JSON string
subscription_group_localization_create_request_instance = SubscriptionGroupLocalizationCreateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupLocalizationCreateRequest.to_json())

# convert the object into a dict
subscription_group_localization_create_request_dict = subscription_group_localization_create_request_instance.to_dict()
# create an instance of SubscriptionGroupLocalizationCreateRequest from a dict
subscription_group_localization_create_request_from_dict = SubscriptionGroupLocalizationCreateRequest.from_dict(subscription_group_localization_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


