# SubscriptionIntroductoryOffersResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionIntroductoryOffer]**](SubscriptionIntroductoryOffer.md) |  | 
**included** | [**List[SubscriptionIntroductoryOffersResponseIncludedInner]**](SubscriptionIntroductoryOffersResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_introductory_offers_response import SubscriptionIntroductoryOffersResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionIntroductoryOffersResponse from a JSON string
subscription_introductory_offers_response_instance = SubscriptionIntroductoryOffersResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionIntroductoryOffersResponse.to_json())

# convert the object into a dict
subscription_introductory_offers_response_dict = subscription_introductory_offers_response_instance.to_dict()
# create an instance of SubscriptionIntroductoryOffersResponse from a dict
subscription_introductory_offers_response_from_dict = SubscriptionIntroductoryOffersResponse.from_dict(subscription_introductory_offers_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


