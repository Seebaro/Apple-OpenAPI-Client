# SubscriptionPricePointsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionPricePoint]**](SubscriptionPricePoint.md) |  | 
**included** | [**List[Territory]**](Territory.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_price_points_response import SubscriptionPricePointsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPricePointsResponse from a JSON string
subscription_price_points_response_instance = SubscriptionPricePointsResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPricePointsResponse.to_json())

# convert the object into a dict
subscription_price_points_response_dict = subscription_price_points_response_instance.to_dict()
# create an instance of SubscriptionPricePointsResponse from a dict
subscription_price_points_response_from_dict = SubscriptionPricePointsResponse.from_dict(subscription_price_points_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


