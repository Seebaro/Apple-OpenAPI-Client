# SubscriptionOfferCodeAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**customer_eligibilities** | [**List[SubscriptionCustomerEligibility]**](SubscriptionCustomerEligibility.md) |  | [optional] 
**offer_eligibility** | [**SubscriptionOfferEligibility**](SubscriptionOfferEligibility.md) |  | [optional] 
**duration** | [**SubscriptionOfferDuration**](SubscriptionOfferDuration.md) |  | [optional] 
**offer_mode** | [**SubscriptionOfferMode**](SubscriptionOfferMode.md) |  | [optional] 
**number_of_periods** | **int** |  | [optional] 
**active** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_attributes import SubscriptionOfferCodeAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeAttributes from a JSON string
subscription_offer_code_attributes_instance = SubscriptionOfferCodeAttributes.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeAttributes.to_json())

# convert the object into a dict
subscription_offer_code_attributes_dict = subscription_offer_code_attributes_instance.to_dict()
# create an instance of SubscriptionOfferCodeAttributes from a dict
subscription_offer_code_attributes_from_dict = SubscriptionOfferCodeAttributes.from_dict(subscription_offer_code_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


