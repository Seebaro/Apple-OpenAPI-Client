# SubscriptionPriceInlineCreateAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**start_date** | **date** |  | [optional] 
**preserve_current_price** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.subscription_price_inline_create_attributes import SubscriptionPriceInlineCreateAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPriceInlineCreateAttributes from a JSON string
subscription_price_inline_create_attributes_instance = SubscriptionPriceInlineCreateAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPriceInlineCreateAttributes.to_json())

# convert the object into a dict
subscription_price_inline_create_attributes_dict = subscription_price_inline_create_attributes_instance.to_dict()
# create an instance of SubscriptionPriceInlineCreateAttributes from a dict
subscription_price_inline_create_attributes_from_dict = SubscriptionPriceInlineCreateAttributes.from_dict(subscription_price_inline_create_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


