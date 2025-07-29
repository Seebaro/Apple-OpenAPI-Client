# SubscriptionIntroductoryOffersLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionRelationshipsIntroductoryOffersDataInner]**](SubscriptionRelationshipsIntroductoryOffersDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_introductory_offers_linkages_response import SubscriptionIntroductoryOffersLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionIntroductoryOffersLinkagesResponse from a JSON string
subscription_introductory_offers_linkages_response_instance = SubscriptionIntroductoryOffersLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionIntroductoryOffersLinkagesResponse.to_json())

# convert the object into a dict
subscription_introductory_offers_linkages_response_dict = subscription_introductory_offers_linkages_response_instance.to_dict()
# create an instance of SubscriptionIntroductoryOffersLinkagesResponse from a dict
subscription_introductory_offers_linkages_response_from_dict = SubscriptionIntroductoryOffersLinkagesResponse.from_dict(subscription_introductory_offers_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


