# SubscriptionOfferCodeOneTimeUseCodeCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**SubscriptionOfferCodeOneTimeUseCodeCreateRequestDataAttributes**](SubscriptionOfferCodeOneTimeUseCodeCreateRequestDataAttributes.md) |  | 
**relationships** | [**SubscriptionOfferCodeCustomCodeCreateRequestDataRelationships**](SubscriptionOfferCodeCustomCodeCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.subscription_offer_code_one_time_use_code_create_request_data import SubscriptionOfferCodeOneTimeUseCodeCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodeOneTimeUseCodeCreateRequestData from a JSON string
subscription_offer_code_one_time_use_code_create_request_data_instance = SubscriptionOfferCodeOneTimeUseCodeCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodeOneTimeUseCodeCreateRequestData.to_json())

# convert the object into a dict
subscription_offer_code_one_time_use_code_create_request_data_dict = subscription_offer_code_one_time_use_code_create_request_data_instance.to_dict()
# create an instance of SubscriptionOfferCodeOneTimeUseCodeCreateRequestData from a dict
subscription_offer_code_one_time_use_code_create_request_data_from_dict = SubscriptionOfferCodeOneTimeUseCodeCreateRequestData.from_dict(subscription_offer_code_one_time_use_code_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


