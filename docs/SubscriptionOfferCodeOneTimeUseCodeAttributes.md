# SubscriptionOfferCodeOneTimeUseCodeAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**number_of_codes** | **int** |  | [optional] 
**created_date** | **datetime** |  | [optional] 
**expiration_date** | **date** |  | [optional] 
**active** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_one_time_use_code_attributes import SubscriptionOfferCodeOneTimeUseCodeAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeOneTimeUseCodeAttributes from a JSON string
subscription_offer_code_one_time_use_code_attributes_instance = SubscriptionOfferCodeOneTimeUseCodeAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeOneTimeUseCodeAttributes.to_json())

# convert the object into a dict
subscription_offer_code_one_time_use_code_attributes_dict = subscription_offer_code_one_time_use_code_attributes_instance.to_dict()
# create an instance of SubscriptionOfferCodeOneTimeUseCodeAttributes from a dict
subscription_offer_code_one_time_use_code_attributes_from_dict = SubscriptionOfferCodeOneTimeUseCodeAttributes.from_dict(subscription_offer_code_one_time_use_code_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


