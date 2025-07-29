# SubscriptionGroupRelationshipsSubscriptionGroupLocalizations


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[SubscriptionGroupRelationshipsSubscriptionGroupLocalizationsDataInner]**](SubscriptionGroupRelationshipsSubscriptionGroupLocalizationsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_group_relationships_subscription_group_localizations import SubscriptionGroupRelationshipsSubscriptionGroupLocalizations

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupRelationshipsSubscriptionGroupLocalizations from a JSON string
subscription_group_relationships_subscription_group_localizations_instance = SubscriptionGroupRelationshipsSubscriptionGroupLocalizations.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupRelationshipsSubscriptionGroupLocalizations.to_json())

# convert the object into a dict
subscription_group_relationships_subscription_group_localizations_dict = subscription_group_relationships_subscription_group_localizations_instance.to_dict()
# create an instance of SubscriptionGroupRelationshipsSubscriptionGroupLocalizations from a dict
subscription_group_relationships_subscription_group_localizations_from_dict = SubscriptionGroupRelationshipsSubscriptionGroupLocalizations.from_dict(subscription_group_relationships_subscription_group_localizations_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


