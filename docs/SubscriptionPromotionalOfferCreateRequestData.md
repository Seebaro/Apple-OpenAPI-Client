# SubscriptionPromotionalOfferCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**SubscriptionPromotionalOfferInlineCreateAttributes**](SubscriptionPromotionalOfferInlineCreateAttributes.md) |  | 
**relationships** | [**SubscriptionPromotionalOfferCreateRequestDataRelationships**](SubscriptionPromotionalOfferCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.subscription_promotional_offer_create_request_data import SubscriptionPromotionalOfferCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotionalOfferCreateRequestData from a JSON string
subscription_promotional_offer_create_request_data_instance = SubscriptionPromotionalOfferCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotionalOfferCreateRequestData.to_json())

# convert the object into a dict
subscription_promotional_offer_create_request_data_dict = subscription_promotional_offer_create_request_data_instance.to_dict()
# create an instance of SubscriptionPromotionalOfferCreateRequestData from a dict
subscription_promotional_offer_create_request_data_from_dict = SubscriptionPromotionalOfferCreateRequestData.from_dict(subscription_promotional_offer_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


