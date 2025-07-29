# SubscriptionOfferCodeOneTimeUseCodeValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_one_time_use_code_value import SubscriptionOfferCodeOneTimeUseCodeValue

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeOneTimeUseCodeValue from a JSON string
subscription_offer_code_one_time_use_code_value_instance = SubscriptionOfferCodeOneTimeUseCodeValue.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeOneTimeUseCodeValue.to_json())

# convert the object into a dict
subscription_offer_code_one_time_use_code_value_dict = subscription_offer_code_one_time_use_code_value_instance.to_dict()
# create an instance of SubscriptionOfferCodeOneTimeUseCodeValue from a dict
subscription_offer_code_one_time_use_code_value_from_dict = SubscriptionOfferCodeOneTimeUseCodeValue.from_dict(subscription_offer_code_one_time_use_code_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


