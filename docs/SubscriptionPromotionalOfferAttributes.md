# SubscriptionPromotionalOfferAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**duration** | [**SubscriptionOfferDuration**](SubscriptionOfferDuration.md) |  | [optional] 
**name** | **str** |  | [optional] 
**number_of_periods** | **int** |  | [optional] 
**offer_code** | **str** |  | [optional] 
**offer_mode** | [**SubscriptionOfferMode**](SubscriptionOfferMode.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_promotional_offer_attributes import SubscriptionPromotionalOfferAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotionalOfferAttributes from a JSON string
subscription_promotional_offer_attributes_instance = SubscriptionPromotionalOfferAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotionalOfferAttributes.to_json())

# convert the object into a dict
subscription_promotional_offer_attributes_dict = subscription_promotional_offer_attributes_instance.to_dict()
# create an instance of SubscriptionPromotionalOfferAttributes from a dict
subscription_promotional_offer_attributes_from_dict = SubscriptionPromotionalOfferAttributes.from_dict(subscription_promotional_offer_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


