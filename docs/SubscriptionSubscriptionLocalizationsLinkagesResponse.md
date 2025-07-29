# SubscriptionSubscriptionLocalizationsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionRelationshipsSubscriptionLocalizationsDataInner]**](SubscriptionRelationshipsSubscriptionLocalizationsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_subscription_localizations_linkages_response import SubscriptionSubscriptionLocalizationsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionSubscriptionLocalizationsLinkagesResponse from a JSON string
subscription_subscription_localizations_linkages_response_instance = SubscriptionSubscriptionLocalizationsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionSubscriptionLocalizationsLinkagesResponse.to_json())

# convert the object into a dict
subscription_subscription_localizations_linkages_response_dict = subscription_subscription_localizations_linkages_response_instance.to_dict()
# create an instance of SubscriptionSubscriptionLocalizationsLinkagesResponse from a dict
subscription_subscription_localizations_linkages_response_from_dict = SubscriptionSubscriptionLocalizationsLinkagesResponse.from_dict(subscription_subscription_localizations_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


