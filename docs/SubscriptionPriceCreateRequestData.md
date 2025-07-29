# SubscriptionPriceCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**SubscriptionPriceInlineCreateAttributes**](SubscriptionPriceInlineCreateAttributes.md) |  | [optional] 
**relationships** | [**SubscriptionPriceCreateRequestDataRelationships**](SubscriptionPriceCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.subscription_price_create_request_data import SubscriptionPriceCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPriceCreateRequestData from a JSON string
subscription_price_create_request_data_instance = SubscriptionPriceCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPriceCreateRequestData.to_json())

# convert the object into a dict
subscription_price_create_request_data_dict = subscription_price_create_request_data_instance.to_dict()
# create an instance of SubscriptionPriceCreateRequestData from a dict
subscription_price_create_request_data_from_dict = SubscriptionPriceCreateRequestData.from_dict(subscription_price_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


