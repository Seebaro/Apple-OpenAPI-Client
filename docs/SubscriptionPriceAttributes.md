# SubscriptionPriceAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**start_date** | **date** |  | [optional] 
**preserved** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.subscription_price_attributes import SubscriptionPriceAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPriceAttributes from a JSON string
subscription_price_attributes_instance = SubscriptionPriceAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPriceAttributes.to_json())

# convert the object into a dict
subscription_price_attributes_dict = subscription_price_attributes_instance.to_dict()
# create an instance of SubscriptionPriceAttributes from a dict
subscription_price_attributes_from_dict = SubscriptionPriceAttributes.from_dict(subscription_price_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


