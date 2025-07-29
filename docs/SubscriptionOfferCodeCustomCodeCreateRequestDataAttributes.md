# SubscriptionOfferCodeCustomCodeCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**custom_code** | **str** |  | 
**number_of_codes** | **int** |  | 
**expiration_date** | **date** |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_custom_code_create_request_data_attributes import SubscriptionOfferCodeCustomCodeCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeCustomCodeCreateRequestDataAttributes from a JSON string
subscription_offer_code_custom_code_create_request_data_attributes_instance = SubscriptionOfferCodeCustomCodeCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeCustomCodeCreateRequestDataAttributes.to_json())

# convert the object into a dict
subscription_offer_code_custom_code_create_request_data_attributes_dict = subscription_offer_code_custom_code_create_request_data_attributes_instance.to_dict()
# create an instance of SubscriptionOfferCodeCustomCodeCreateRequestDataAttributes from a dict
subscription_offer_code_custom_code_create_request_data_attributes_from_dict = SubscriptionOfferCodeCustomCodeCreateRequestDataAttributes.from_dict(subscription_offer_code_custom_code_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


