# SubscriptionPricePointResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionPricePoint**](SubscriptionPricePoint.md) |  | 
**included** | [**List[Territory]**](Territory.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_price_point_response import SubscriptionPricePointResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPricePointResponse from a JSON string
subscription_price_point_response_instance = SubscriptionPricePointResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPricePointResponse.to_json())

# convert the object into a dict
subscription_price_point_response_dict = subscription_price_point_response_instance.to_dict()
# create an instance of SubscriptionPricePointResponse from a dict
subscription_price_point_response_from_dict = SubscriptionPricePointResponse.from_dict(subscription_price_point_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


