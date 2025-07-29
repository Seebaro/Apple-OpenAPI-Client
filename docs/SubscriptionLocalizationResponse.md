# SubscriptionLocalizationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionLocalization**](SubscriptionLocalization.md) |  | 
**included** | [**List[Subscription]**](Subscription.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_localization_response import SubscriptionLocalizationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionLocalizationResponse from a JSON string
subscription_localization_response_instance = SubscriptionLocalizationResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionLocalizationResponse.to_json())

# convert the object into a dict
subscription_localization_response_dict = subscription_localization_response_instance.to_dict()
# create an instance of SubscriptionLocalizationResponse from a dict
subscription_localization_response_from_dict = SubscriptionLocalizationResponse.from_dict(subscription_localization_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


