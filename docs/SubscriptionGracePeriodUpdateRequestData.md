# SubscriptionGracePeriodUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionGracePeriodAttributes**](SubscriptionGracePeriodAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_grace_period_update_request_data import SubscriptionGracePeriodUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGracePeriodUpdateRequestData from a JSON string
subscription_grace_period_update_request_data_instance = SubscriptionGracePeriodUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGracePeriodUpdateRequestData.to_json())

# convert the object into a dict
subscription_grace_period_update_request_data_dict = subscription_grace_period_update_request_data_instance.to_dict()
# create an instance of SubscriptionGracePeriodUpdateRequestData from a dict
subscription_grace_period_update_request_data_from_dict = SubscriptionGracePeriodUpdateRequestData.from_dict(subscription_grace_period_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


