# SubscriptionOfferCodeCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**customer_eligibilities** | [**List[SubscriptionCustomerEligibility]**](SubscriptionCustomerEligibility.md) |  | 
**offer_eligibility** | [**SubscriptionOfferEligibility**](SubscriptionOfferEligibility.md) |  | 
**duration** | [**SubscriptionOfferDuration**](SubscriptionOfferDuration.md) |  | 
**offer_mode** | [**SubscriptionOfferMode**](SubscriptionOfferMode.md) |  | 
**number_of_periods** | **int** |  | 

## Example

```python
from openapi_client.models.subscription_offer_code_create_request_data_attributes import SubscriptionOfferCodeCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeCreateRequestDataAttributes from a JSON string
subscription_offer_code_create_request_data_attributes_instance = SubscriptionOfferCodeCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeCreateRequestDataAttributes.to_json())

# convert the object into a dict
subscription_offer_code_create_request_data_attributes_dict = subscription_offer_code_create_request_data_attributes_instance.to_dict()
# create an instance of SubscriptionOfferCodeCreateRequestDataAttributes from a dict
subscription_offer_code_create_request_data_attributes_from_dict = SubscriptionOfferCodeCreateRequestDataAttributes.from_dict(subscription_offer_code_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


