# SubscriptionPromotionalOffersResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionPromotionalOffer]**](SubscriptionPromotionalOffer.md) |  | 
**included** | [**List[SubscriptionPromotionalOffersResponseIncludedInner]**](SubscriptionPromotionalOffersResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_promotional_offers_response import SubscriptionPromotionalOffersResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotionalOffersResponse from a JSON string
subscription_promotional_offers_response_instance = SubscriptionPromotionalOffersResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotionalOffersResponse.to_json())

# convert the object into a dict
subscription_promotional_offers_response_dict = subscription_promotional_offers_response_instance.to_dict()
# create an instance of SubscriptionPromotionalOffersResponse from a dict
subscription_promotional_offers_response_from_dict = SubscriptionPromotionalOffersResponse.from_dict(subscription_promotional_offers_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


