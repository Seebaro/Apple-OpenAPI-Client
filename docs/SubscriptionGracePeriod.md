# SubscriptionGracePeriod


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionGracePeriodAttributes**](SubscriptionGracePeriodAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_grace_period import SubscriptionGracePeriod

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGracePeriod from a JSON string
subscription_grace_period_instance = SubscriptionGracePeriod.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGracePeriod.to_json())

# convert the object into a dict
subscription_grace_period_dict = subscription_grace_period_instance.to_dict()
# create an instance of SubscriptionGracePeriod from a dict
subscription_grace_period_from_dict = SubscriptionGracePeriod.from_dict(subscription_grace_period_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


