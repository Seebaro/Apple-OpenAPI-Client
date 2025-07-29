# SubscriptionPricesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionRelationshipsPricesDataInner]**](SubscriptionRelationshipsPricesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_prices_linkages_response import SubscriptionPricesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPricesLinkagesResponse from a JSON string
subscription_prices_linkages_response_instance = SubscriptionPricesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPricesLinkagesResponse.to_json())

# convert the object into a dict
subscription_prices_linkages_response_dict = subscription_prices_linkages_response_instance.to_dict()
# create an instance of SubscriptionPricesLinkagesResponse from a dict
subscription_prices_linkages_response_from_dict = SubscriptionPricesLinkagesResponse.from_dict(subscription_prices_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


