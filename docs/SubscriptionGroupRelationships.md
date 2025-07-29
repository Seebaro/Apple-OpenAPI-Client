# SubscriptionGroupRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subscriptions** | [**SubscriptionGroupRelationshipsSubscriptions**](SubscriptionGroupRelationshipsSubscriptions.md) |  | [optional] 
**subscription_group_localizations** | [**SubscriptionGroupRelationshipsSubscriptionGroupLocalizations**](SubscriptionGroupRelationshipsSubscriptionGroupLocalizations.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_group_relationships import SubscriptionGroupRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupRelationships from a JSON string
subscription_group_relationships_instance = SubscriptionGroupRelationships.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupRelationships.to_json())

# convert the object into a dict
subscription_group_relationships_dict = subscription_group_relationships_instance.to_dict()
# create an instance of SubscriptionGroupRelationships from a dict
subscription_group_relationships_from_dict = SubscriptionGroupRelationships.from_dict(subscription_group_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


