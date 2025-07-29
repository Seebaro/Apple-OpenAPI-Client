# SubscriptionPromotionalOffersResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionAttributes**](SubscriptionAttributes.md) |  | [optional] 
**relationships** | [**SubscriptionOfferCodePriceRelationships**](SubscriptionOfferCodePriceRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_promotional_offers_response_included_inner import SubscriptionPromotionalOffersResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionPromotionalOffersResponseIncludedInner from a JSON string
subscription_promotional_offers_response_included_inner_instance = SubscriptionPromotionalOffersResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(SubscriptionPromotionalOffersResponseIncludedInner.to_json())

# convert the object into a dict
subscription_promotional_offers_response_included_inner_dict = subscription_promotional_offers_response_included_inner_instance.to_dict()
# create an instance of SubscriptionPromotionalOffersResponseIncludedInner from a dict
subscription_promotional_offers_response_included_inner_from_dict = SubscriptionPromotionalOffersResponseIncludedInner.from_dict(subscription_promotional_offers_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


