# SubscriptionOfferCodeCustomCode


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionOfferCodeCustomCodeAttributes**](SubscriptionOfferCodeCustomCodeAttributes.md) |  | [optional] 
**relationships** | [**SubscriptionOfferCodeCustomCodeRelationships**](SubscriptionOfferCodeCustomCodeRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_custom_code import SubscriptionOfferCodeCustomCode

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeCustomCode from a JSON string
subscription_offer_code_custom_code_instance = SubscriptionOfferCodeCustomCode.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeCustomCode.to_json())

# convert the object into a dict
subscription_offer_code_custom_code_dict = subscription_offer_code_custom_code_instance.to_dict()
# create an instance of SubscriptionOfferCodeCustomCode from a dict
subscription_offer_code_custom_code_from_dict = SubscriptionOfferCodeCustomCode.from_dict(subscription_offer_code_custom_code_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


