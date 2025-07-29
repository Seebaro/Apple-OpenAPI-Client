# SubscriptionOfferCodeOneTimeUseCodeUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionOfferCodeCustomCodeUpdateRequestDataAttributes**](SubscriptionOfferCodeCustomCodeUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_code_one_time_use_code_update_request_data import SubscriptionOfferCodeOneTimeUseCodeUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeOneTimeUseCodeUpdateRequestData from a JSON string
subscription_offer_code_one_time_use_code_update_request_data_instance = SubscriptionOfferCodeOneTimeUseCodeUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeOneTimeUseCodeUpdateRequestData.to_json())

# convert the object into a dict
subscription_offer_code_one_time_use_code_update_request_data_dict = subscription_offer_code_one_time_use_code_update_request_data_instance.to_dict()
# create an instance of SubscriptionOfferCodeOneTimeUseCodeUpdateRequestData from a dict
subscription_offer_code_one_time_use_code_update_request_data_from_dict = SubscriptionOfferCodeOneTimeUseCodeUpdateRequestData.from_dict(subscription_offer_code_one_time_use_code_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


