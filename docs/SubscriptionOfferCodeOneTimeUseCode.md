# SubscriptionOfferCodeOneTimeUseCode


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionOfferCodeOneTimeUseCodeAttributes**](SubscriptionOfferCodeOneTimeUseCodeAttributes.md) |  | [optional] 
**relationships** | [**SubscriptionOfferCodeOneTimeUseCodeRelationships**](SubscriptionOfferCodeOneTimeUseCodeRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_one_time_use_code import SubscriptionOfferCodeOneTimeUseCode

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeOneTimeUseCode from a JSON string
subscription_offer_code_one_time_use_code_instance = SubscriptionOfferCodeOneTimeUseCode.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeOneTimeUseCode.to_json())

# convert the object into a dict
subscription_offer_code_one_time_use_code_dict = subscription_offer_code_one_time_use_code_instance.to_dict()
# create an instance of SubscriptionOfferCodeOneTimeUseCode from a dict
subscription_offer_code_one_time_use_code_from_dict = SubscriptionOfferCodeOneTimeUseCode.from_dict(subscription_offer_code_one_time_use_code_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


