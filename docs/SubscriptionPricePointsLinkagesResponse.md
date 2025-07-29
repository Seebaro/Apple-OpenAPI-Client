# SubscriptionPricePointsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionIntroductoryOfferRelationshipsSubscriptionPricePointData]**](SubscriptionIntroductoryOfferRelationshipsSubscriptionPricePointData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_price_points_linkages_response import SubscriptionPricePointsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPricePointsLinkagesResponse from a JSON string
subscription_price_points_linkages_response_instance = SubscriptionPricePointsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPricePointsLinkagesResponse.to_json())

# convert the object into a dict
subscription_price_points_linkages_response_dict = subscription_price_points_linkages_response_instance.to_dict()
# create an instance of SubscriptionPricePointsLinkagesResponse from a dict
subscription_price_points_linkages_response_from_dict = SubscriptionPricePointsLinkagesResponse.from_dict(subscription_price_points_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


