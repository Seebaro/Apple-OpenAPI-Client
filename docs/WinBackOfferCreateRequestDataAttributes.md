# WinBackOfferCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | 
**offer_id** | **str** |  | 
**duration** | [**SubscriptionOfferDuration**](SubscriptionOfferDuration.md) |  | 
**offer_mode** | [**SubscriptionOfferMode**](SubscriptionOfferMode.md) |  | 
**period_count** | **int** |  | 
**customer_eligibility_paid_subscription_duration_in_months** | **int** |  | 
**customer_eligibility_time_since_last_subscribed_in_months** | [**IntegerRange**](IntegerRange.md) |  | 
**customer_eligibility_wait_between_offers_in_months** | **int** |  | [optional] 
**start_date** | **date** |  | 
**end_date** | **date** |  | [optional] 
**priority** | **str** |  | 
**promotion_intent** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.win_back_offer_create_request_data_attributes import WinBackOfferCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of WinBackOfferCreateRequestDataAttributes from a JSON string
win_back_offer_create_request_data_attributes_instance = WinBackOfferCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(WinBackOfferCreateRequestDataAttributes.to_json())

# convert the object into a dict
win_back_offer_create_request_data_attributes_dict = win_back_offer_create_request_data_attributes_instance.to_dict()
# create an instance of WinBackOfferCreateRequestDataAttributes from a dict
win_back_offer_create_request_data_attributes_from_dict = WinBackOfferCreateRequestDataAttributes.from_dict(win_back_offer_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


