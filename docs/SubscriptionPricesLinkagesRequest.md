# SubscriptionPricesLinkagesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionRelationshipsPricesDataInner]**](SubscriptionRelationshipsPricesDataInner.md) |  | 

## Example

```python
from openapi_client.models.subscription_prices_linkages_request import SubscriptionPricesLinkagesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPricesLinkagesRequest from a JSON string
subscription_prices_linkages_request_instance = SubscriptionPricesLinkagesRequest.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPricesLinkagesRequest.to_json())

# convert the object into a dict
subscription_prices_linkages_request_dict = subscription_prices_linkages_request_instance.to_dict()
# create an instance of SubscriptionPricesLinkagesRequest from a dict
subscription_prices_linkages_request_from_dict = SubscriptionPricesLinkagesRequest.from_dict(subscription_prices_linkages_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


