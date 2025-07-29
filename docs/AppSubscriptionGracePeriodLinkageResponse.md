# AppSubscriptionGracePeriodLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppRelationshipsSubscriptionGracePeriodData**](AppRelationshipsSubscriptionGracePeriodData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_subscription_grace_period_linkage_response import AppSubscriptionGracePeriodLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppSubscriptionGracePeriodLinkageResponse from a JSON string
app_subscription_grace_period_linkage_response_instance = AppSubscriptionGracePeriodLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppSubscriptionGracePeriodLinkageResponse.to_json())

# convert the object into a dict
app_subscription_grace_period_linkage_response_dict = app_subscription_grace_period_linkage_response_instance.to_dict()
# create an instance of AppSubscriptionGracePeriodLinkageResponse from a dict
app_subscription_grace_period_linkage_response_from_dict = AppSubscriptionGracePeriodLinkageResponse.from_dict(app_subscription_grace_period_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


