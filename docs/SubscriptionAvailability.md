# SubscriptionAvailability


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppAvailabilityV2Attributes**](AppAvailabilityV2Attributes.md) |  | [optional] 
**relationships** | [**InAppPurchaseAvailabilityRelationships**](InAppPurchaseAvailabilityRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_availability import SubscriptionAvailability

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionAvailability from a JSON string
subscription_availability_instance = SubscriptionAvailability.from_json(json)
# print the JSON string representation of the object
print(SubscriptionAvailability.to_json())

# convert the object into a dict
subscription_availability_dict = subscription_availability_instance.to_dict()
# create an instance of SubscriptionAvailability from a dict
subscription_availability_from_dict = SubscriptionAvailability.from_dict(subscription_availability_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


