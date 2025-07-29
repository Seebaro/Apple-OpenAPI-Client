# SubscriptionRelationshipsSubscriptionAvailability


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**data** | [**SubscriptionRelationshipsSubscriptionAvailabilityData**](SubscriptionRelationshipsSubscriptionAvailabilityData.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_relationships_subscription_availability import SubscriptionRelationshipsSubscriptionAvailability

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionRelationshipsSubscriptionAvailability from a JSON string
subscription_relationships_subscription_availability_instance = SubscriptionRelationshipsSubscriptionAvailability.from_json(json)
# print the JSON string representation of the object
print(SubscriptionRelationshipsSubscriptionAvailability.to_json())

# convert the object into a dict
subscription_relationships_subscription_availability_dict = subscription_relationships_subscription_availability_instance.to_dict()
# create an instance of SubscriptionRelationshipsSubscriptionAvailability from a dict
subscription_relationships_subscription_availability_from_dict = SubscriptionRelationshipsSubscriptionAvailability.from_dict(subscription_relationships_subscription_availability_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


