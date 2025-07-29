# SubscriptionGroupSubscriptionsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[PromotedPurchaseRelationshipsSubscriptionData]**](PromotedPurchaseRelationshipsSubscriptionData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_group_subscriptions_linkages_response import SubscriptionGroupSubscriptionsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionGroupSubscriptionsLinkagesResponse from a JSON string
subscription_group_subscriptions_linkages_response_instance = SubscriptionGroupSubscriptionsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionGroupSubscriptionsLinkagesResponse.to_json())

# convert the object into a dict
subscription_group_subscriptions_linkages_response_dict = subscription_group_subscriptions_linkages_response_instance.to_dict()
# create an instance of SubscriptionGroupSubscriptionsLinkagesResponse from a dict
subscription_group_subscriptions_linkages_response_from_dict = SubscriptionGroupSubscriptionsLinkagesResponse.from_dict(subscription_group_subscriptions_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


