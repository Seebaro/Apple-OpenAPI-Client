# SubscriptionPricePoint


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionPricePointAttributes**](SubscriptionPricePointAttributes.md) |  | [optional] 
**relationships** | [**InAppPurchasePricePointRelationships**](InAppPurchasePricePointRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_price_point import SubscriptionPricePoint

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPricePoint from a JSON string
subscription_price_point_instance = SubscriptionPricePoint.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPricePoint.to_json())

# convert the object into a dict
subscription_price_point_dict = subscription_price_point_instance.to_dict()
# create an instance of SubscriptionPricePoint from a dict
subscription_price_point_from_dict = SubscriptionPricePoint.from_dict(subscription_price_point_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


