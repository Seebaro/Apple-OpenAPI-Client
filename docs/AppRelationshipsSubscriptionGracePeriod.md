# AppRelationshipsSubscriptionGracePeriod


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**data** | [**AppRelationshipsSubscriptionGracePeriodData**](AppRelationshipsSubscriptionGracePeriodData.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_relationships_subscription_grace_period import AppRelationshipsSubscriptionGracePeriod

# TODO update the JSON string below
json = "{}"
# create an instance of AppRelationshipsSubscriptionGracePeriod from a JSON string
app_relationships_subscription_grace_period_instance = AppRelationshipsSubscriptionGracePeriod.from_json(json)
# print the JSON string representation of the object
print(AppRelationshipsSubscriptionGracePeriod.to_json())

# convert the object into a dict
app_relationships_subscription_grace_period_dict = app_relationships_subscription_grace_period_instance.to_dict()
# create an instance of AppRelationshipsSubscriptionGracePeriod from a dict
app_relationships_subscription_grace_period_from_dict = AppRelationshipsSubscriptionGracePeriod.from_dict(app_relationships_subscription_grace_period_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


