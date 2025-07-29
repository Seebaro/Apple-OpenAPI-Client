# WinBackOfferUpdateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_eligibility_paid_subscription_duration_in_months** | **int** |  | [optional] 
**customer_eligibility_time_since_last_subscribed_in_months** | [**IntegerRange**](IntegerRange.md) |  | [optional] 
**customer_eligibility_wait_between_offers_in_months** | **int** |  | [optional] 
**start_date** | **date** |  | [optional] 
**end_date** | **date** |  | [optional] 
**priority** | **str** |  | [optional] 
**promotion_intent** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.win_back_offer_update_request_data_attributes import WinBackOfferUpdateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of WinBackOfferUpdateRequestDataAttributes from a JSON string
win_back_offer_update_request_data_attributes_instance = WinBackOfferUpdateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(WinBackOfferUpdateRequestDataAttributes.to_json())

# convert the object into a dict
win_back_offer_update_request_data_attributes_dict = win_back_offer_update_request_data_attributes_instance.to_dict()
# create an instance of WinBackOfferUpdateRequestDataAttributes from a dict
win_back_offer_update_request_data_attributes_from_dict = WinBackOfferUpdateRequestDataAttributes.from_dict(win_back_offer_update_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


