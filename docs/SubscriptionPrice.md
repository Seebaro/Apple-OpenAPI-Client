# SubscriptionPrice


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionPriceAttributes**](SubscriptionPriceAttributes.md) |  | [optional] 
**relationships** | [**SubscriptionOfferCodePriceRelationships**](SubscriptionOfferCodePriceRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_price import SubscriptionPrice

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPrice from a JSON string
subscription_price_instance = SubscriptionPrice.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPrice.to_json())

# convert the object into a dict
subscription_price_dict = subscription_price_instance.to_dict()
# create an instance of SubscriptionPrice from a dict
subscription_price_from_dict = SubscriptionPrice.from_dict(subscription_price_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


