# SubscriptionOfferCodeCustomCodeAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**custom_code** | **str** |  | [optional] 
**number_of_codes** | **int** |  | [optional] 
**created_date** | **datetime** |  | [optional] 
**expiration_date** | **date** |  | [optional] 
**active** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_custom_code_attributes import SubscriptionOfferCodeCustomCodeAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeCustomCodeAttributes from a JSON string
subscription_offer_code_custom_code_attributes_instance = SubscriptionOfferCodeCustomCodeAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeCustomCodeAttributes.to_json())

# convert the object into a dict
subscription_offer_code_custom_code_attributes_dict = subscription_offer_code_custom_code_attributes_instance.to_dict()
# create an instance of SubscriptionOfferCodeCustomCodeAttributes from a dict
subscription_offer_code_custom_code_attributes_from_dict = SubscriptionOfferCodeCustomCodeAttributes.from_dict(subscription_offer_code_custom_code_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


