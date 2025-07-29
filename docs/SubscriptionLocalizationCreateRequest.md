# SubscriptionLocalizationCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionLocalizationCreateRequestData**](SubscriptionLocalizationCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.subscription_localization_create_request import SubscriptionLocalizationCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionLocalizationCreateRequest from a JSON string
subscription_localization_create_request_instance = SubscriptionLocalizationCreateRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionLocalizationCreateRequest.to_json())

# convert the object into a dict
subscription_localization_create_request_dict = subscription_localization_create_request_instance.to_dict()
# create an instance of SubscriptionLocalizationCreateRequest from a dict
subscription_localization_create_request_from_dict = SubscriptionLocalizationCreateRequest.from_dict(subscription_localization_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


