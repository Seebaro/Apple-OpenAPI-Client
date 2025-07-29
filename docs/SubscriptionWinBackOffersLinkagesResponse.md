# SubscriptionWinBackOffersLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionRelationshipsWinBackOffersDataInner]**](SubscriptionRelationshipsWinBackOffersDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_win_back_offers_linkages_response import SubscriptionWinBackOffersLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionWinBackOffersLinkagesResponse from a JSON string
subscription_win_back_offers_linkages_response_instance = SubscriptionWinBackOffersLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionWinBackOffersLinkagesResponse.to_json())

# convert the object into a dict
subscription_win_back_offers_linkages_response_dict = subscription_win_back_offers_linkages_response_instance.to_dict()
# create an instance of SubscriptionWinBackOffersLinkagesResponse from a dict
subscription_win_back_offers_linkages_response_from_dict = SubscriptionWinBackOffersLinkagesResponse.from_dict(subscription_win_back_offers_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


