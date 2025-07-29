# SubscriptionGroupsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionGroup]**](SubscriptionGroup.md) |  | 
**included** | [**List[SubscriptionGroupsResponseIncludedInner]**](SubscriptionGroupsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_groups_response import SubscriptionGroupsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupsResponse from a JSON string
subscription_groups_response_instance = SubscriptionGroupsResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupsResponse.to_json())

# convert the object into a dict
subscription_groups_response_dict = subscription_groups_response_instance.to_dict()
# create an instance of SubscriptionGroupsResponse from a dict
subscription_groups_response_from_dict = SubscriptionGroupsResponse.from_dict(subscription_groups_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


