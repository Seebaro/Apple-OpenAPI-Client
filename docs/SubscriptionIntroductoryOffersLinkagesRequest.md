# SubscriptionIntroductoryOffersLinkagesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionRelationshipsIntroductoryOffersDataInner]**](SubscriptionRelationshipsIntroductoryOffersDataInner.md) |  | 

## Example

```python
from openapi_client.models.subscription_introductory_offers_linkages_request import SubscriptionIntroductoryOffersLinkagesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionIntroductoryOffersLinkagesRequest from a JSON string
subscription_introductory_offers_linkages_request_instance = SubscriptionIntroductoryOffersLinkagesRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionIntroductoryOffersLinkagesRequest.to_json())

# convert the object into a dict
subscription_introductory_offers_linkages_request_dict = subscription_introductory_offers_linkages_request_instance.to_dict()
# create an instance of SubscriptionIntroductoryOffersLinkagesRequest from a dict
subscription_introductory_offers_linkages_request_from_dict = SubscriptionIntroductoryOffersLinkagesRequest.from_dict(subscription_introductory_offers_linkages_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


