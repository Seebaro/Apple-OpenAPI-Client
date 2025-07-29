# SubscriptionPricePointAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_price** | **str** |  | [optional] 
**proceeds** | **str** |  | [optional] 
**proceeds_year2** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.subscription_price_point_attributes import SubscriptionPricePointAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPricePointAttributes from a JSON string
subscription_price_point_attributes_instance = SubscriptionPricePointAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPricePointAttributes.to_json())

# convert the object into a dict
subscription_price_point_attributes_dict = subscription_price_point_attributes_instance.to_dict()
# create an instance of SubscriptionPricePointAttributes from a dict
subscription_price_point_attributes_from_dict = SubscriptionPricePointAttributes.from_dict(subscription_price_point_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


