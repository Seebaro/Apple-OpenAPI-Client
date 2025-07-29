# AppSubscriptionGroupsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppRelationshipsSubscriptionGroupsDataInner]**](AppRelationshipsSubscriptionGroupsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_subscription_groups_linkages_response import AppSubscriptionGroupsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppSubscriptionGroupsLinkagesResponse from a JSON string
app_subscription_groups_linkages_response_instance = AppSubscriptionGroupsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppSubscriptionGroupsLinkagesResponse.to_json())

# convert the object into a dict
app_subscription_groups_linkages_response_dict = app_subscription_groups_linkages_response_instance.to_dict()
# create an instance of AppSubscriptionGroupsLinkagesResponse from a dict
app_subscription_groups_linkages_response_from_dict = AppSubscriptionGroupsLinkagesResponse.from_dict(app_subscription_groups_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


