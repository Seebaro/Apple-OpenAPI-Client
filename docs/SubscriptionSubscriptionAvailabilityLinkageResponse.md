# SubscriptionSubscriptionAvailabilityLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionRelationshipsSubscriptionAvailabilityData**](SubscriptionRelationshipsSubscriptionAvailabilityData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_subscription_availability_linkage_response import SubscriptionSubscriptionAvailabilityLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionSubscriptionAvailabilityLinkageResponse from a JSON string
subscription_subscription_availability_linkage_response_instance = SubscriptionSubscriptionAvailabilityLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionSubscriptionAvailabilityLinkageResponse.to_json())

# convert the object into a dict
subscription_subscription_availability_linkage_response_dict = subscription_subscription_availability_linkage_response_instance.to_dict()
# create an instance of SubscriptionSubscriptionAvailabilityLinkageResponse from a dict
subscription_subscription_availability_linkage_response_from_dict = SubscriptionSubscriptionAvailabilityLinkageResponse.from_dict(subscription_subscription_availability_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


