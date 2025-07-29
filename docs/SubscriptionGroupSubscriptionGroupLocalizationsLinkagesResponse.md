# SubscriptionGroupSubscriptionGroupLocalizationsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionGroupRelationshipsSubscriptionGroupLocalizationsDataInner]**](SubscriptionGroupRelationshipsSubscriptionGroupLocalizationsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_group_subscription_group_localizations_linkages_response import SubscriptionGroupSubscriptionGroupLocalizationsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupSubscriptionGroupLocalizationsLinkagesResponse from a JSON string
subscription_group_subscription_group_localizations_linkages_response_instance = SubscriptionGroupSubscriptionGroupLocalizationsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupSubscriptionGroupLocalizationsLinkagesResponse.to_json())

# convert the object into a dict
subscription_group_subscription_group_localizations_linkages_response_dict = subscription_group_subscription_group_localizations_linkages_response_instance.to_dict()
# create an instance of SubscriptionGroupSubscriptionGroupLocalizationsLinkagesResponse from a dict
subscription_group_subscription_group_localizations_linkages_response_from_dict = SubscriptionGroupSubscriptionGroupLocalizationsLinkagesResponse.from_dict(subscription_group_subscription_group_localizations_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


