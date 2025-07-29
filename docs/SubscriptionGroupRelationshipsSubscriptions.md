# SubscriptionGroupRelationshipsSubscriptions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[PromotedPurchaseRelationshipsSubscriptionData]**](PromotedPurchaseRelationshipsSubscriptionData.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_group_relationships_subscriptions import SubscriptionGroupRelationshipsSubscriptions

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupRelationshipsSubscriptions from a JSON string
subscription_group_relationships_subscriptions_instance = SubscriptionGroupRelationshipsSubscriptions.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupRelationshipsSubscriptions.to_json())

# convert the object into a dict
subscription_group_relationships_subscriptions_dict = subscription_group_relationships_subscriptions_instance.to_dict()
# create an instance of SubscriptionGroupRelationshipsSubscriptions from a dict
subscription_group_relationships_subscriptions_from_dict = SubscriptionGroupRelationshipsSubscriptions.from_dict(subscription_group_relationships_subscriptions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


