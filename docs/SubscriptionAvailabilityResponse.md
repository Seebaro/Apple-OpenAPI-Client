# SubscriptionAvailabilityResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionAvailability**](SubscriptionAvailability.md) |  | 
**included** | [**List[Territory]**](Territory.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_availability_response import SubscriptionAvailabilityResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionAvailabilityResponse from a JSON string
subscription_availability_response_instance = SubscriptionAvailabilityResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionAvailabilityResponse.to_json())

# convert the object into a dict
subscription_availability_response_dict = subscription_availability_response_instance.to_dict()
# create an instance of SubscriptionAvailabilityResponse from a dict
subscription_availability_response_from_dict = SubscriptionAvailabilityResponse.from_dict(subscription_availability_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


