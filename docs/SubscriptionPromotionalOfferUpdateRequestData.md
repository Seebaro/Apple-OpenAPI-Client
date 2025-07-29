# SubscriptionPromotionalOfferUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**relationships** | [**SubscriptionPromotionalOfferUpdateRequestDataRelationships**](SubscriptionPromotionalOfferUpdateRequestDataRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_promotional_offer_update_request_data import SubscriptionPromotionalOfferUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotionalOfferUpdateRequestData from a JSON string
subscription_promotional_offer_update_request_data_instance = SubscriptionPromotionalOfferUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotionalOfferUpdateRequestData.to_json())

# convert the object into a dict
subscription_promotional_offer_update_request_data_dict = subscription_promotional_offer_update_request_data_instance.to_dict()
# create an instance of SubscriptionPromotionalOfferUpdateRequestData from a dict
subscription_promotional_offer_update_request_data_from_dict = SubscriptionPromotionalOfferUpdateRequestData.from_dict(subscription_promotional_offer_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


