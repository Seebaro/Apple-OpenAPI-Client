# SubscriptionGracePeriodResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionGracePeriod**](SubscriptionGracePeriod.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_grace_period_response import SubscriptionGracePeriodResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGracePeriodResponse from a JSON string
subscription_grace_period_response_instance = SubscriptionGracePeriodResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGracePeriodResponse.to_json())

# convert the object into a dict
subscription_grace_period_response_dict = subscription_grace_period_response_instance.to_dict()
# create an instance of SubscriptionGracePeriodResponse from a dict
subscription_grace_period_response_from_dict = SubscriptionGracePeriodResponse.from_dict(subscription_grace_period_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


