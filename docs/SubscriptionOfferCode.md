# SubscriptionOfferCode


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionOfferCodeAttributes**](SubscriptionOfferCodeAttributes.md) |  | [optional] 
**relationships** | [**SubscriptionOfferCodeRelationships**](SubscriptionOfferCodeRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code import SubscriptionOfferCode

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCode from a JSON string
subscription_offer_code_instance = SubscriptionOfferCode.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCode.to_json())

# convert the object into a dict
subscription_offer_code_dict = subscription_offer_code_instance.to_dict()
# create an instance of SubscriptionOfferCode from a dict
subscription_offer_code_from_dict = SubscriptionOfferCode.from_dict(subscription_offer_code_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


