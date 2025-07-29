# SubscriptionRelationshipsSubscriptionLocalizations


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[SubscriptionRelationshipsSubscriptionLocalizationsDataInner]**](SubscriptionRelationshipsSubscriptionLocalizationsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_relationships_subscription_localizations import SubscriptionRelationshipsSubscriptionLocalizations

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionRelationshipsSubscriptionLocalizations from a JSON string
subscription_relationships_subscription_localizations_instance = SubscriptionRelationshipsSubscriptionLocalizations.from_json(json)
# print the JSON string representation of the object
print(SubscriptionRelationshipsSubscriptionLocalizations.to_json())

# convert the object into a dict
subscription_relationships_subscription_localizations_dict = subscription_relationships_subscription_localizations_instance.to_dict()
# create an instance of SubscriptionRelationshipsSubscriptionLocalizations from a dict
subscription_relationships_subscription_localizations_from_dict = SubscriptionRelationshipsSubscriptionLocalizations.from_dict(subscription_relationships_subscription_localizations_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


