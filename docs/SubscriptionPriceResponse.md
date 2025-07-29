# SubscriptionPriceResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionPrice**](SubscriptionPrice.md) |  | 
**included** | [**List[SubscriptionOfferCodePricesResponseIncludedInner]**](SubscriptionOfferCodePricesResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_price_response import SubscriptionPriceResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPriceResponse from a JSON string
subscription_price_response_instance = SubscriptionPriceResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPriceResponse.to_json())

# convert the object into a dict
subscription_price_response_dict = subscription_price_response_instance.to_dict()
# create an instance of SubscriptionPriceResponse from a dict
subscription_price_response_from_dict = SubscriptionPriceResponse.from_dict(subscription_price_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


