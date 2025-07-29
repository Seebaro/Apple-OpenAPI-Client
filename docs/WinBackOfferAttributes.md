# WinBackOfferAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | [optional] 
**offer_id** | **str** |  | [optional] 
**duration** | [**SubscriptionOfferDuration**](SubscriptionOfferDuration.md) |  | [optional] 
**offer_mode** | [**SubscriptionOfferMode**](SubscriptionOfferMode.md) |  | [optional] 
**period_count** | **int** |  | [optional] 
**customer_eligibility_paid_subscription_duration_in_months** | **int** |  | [optional] 
**customer_eligibility_time_since_last_subscribed_in_months** | [**IntegerRange**](IntegerRange.md) |  | [optional] 
**customer_eligibility_wait_between_offers_in_months** | **int** |  | [optional] 
**start_date** | **date** |  | [optional] 
**end_date** | **date** |  | [optional] 
**priority** | **str** |  | [optional] 
**promotion_intent** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.win_back_offer_attributes import WinBackOfferAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of WinBackOfferAttributes from a JSON string
win_back_offer_attributes_instance = WinBackOfferAttributes.from_json(json)
# print the JSON string representation of the object
print(WinBackOfferAttributes.to_json())

# convert the object into a dict
win_back_offer_attributes_dict = win_back_offer_attributes_instance.to_dict()
# create an instance of WinBackOfferAttributes from a dict
win_back_offer_attributes_from_dict = WinBackOfferAttributes.from_dict(win_back_offer_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


