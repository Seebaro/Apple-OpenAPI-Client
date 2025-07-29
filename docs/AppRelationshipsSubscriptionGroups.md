# AppRelationshipsSubscriptionGroups


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppRelationshipsSubscriptionGroupsDataInner]**](AppRelationshipsSubscriptionGroupsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_relationships_subscription_groups import AppRelationshipsSubscriptionGroups

# TODO update the JSON string below
json = "{}"
# create an instance of AppRelationshipsSubscriptionGroups from a JSON string
app_relationships_subscription_groups_instance = AppRelationshipsSubscriptionGroups.from_json(json)
# print the JSON string representation of the object
print(AppRelationshipsSubscriptionGroups.to_json())

# convert the object into a dict
app_relationships_subscription_groups_dict = app_relationships_subscription_groups_instance.to_dict()
# create an instance of AppRelationshipsSubscriptionGroups from a dict
app_relationships_subscription_groups_from_dict = AppRelationshipsSubscriptionGroups.from_dict(app_relationships_subscription_groups_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


