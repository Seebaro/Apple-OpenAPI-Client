# SubscriptionOfferCodesResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionOfferCodeCustomCodeAttributes**](SubscriptionOfferCodeCustomCodeAttributes.md) |  | [optional] 
**relationships** | [**SubscriptionOfferCodePriceRelationships**](SubscriptionOfferCodePriceRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_offer_codes_response_included_inner import SubscriptionOfferCodesResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOfferCodesResponseIncludedInner from a JSON string
subscription_offer_codes_response_included_inner_instance = SubscriptionOfferCodesResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOfferCodesResponseIncludedInner.to_json())

# convert the object into a dict
subscription_offer_codes_response_included_inner_dict = subscription_offer_codes_response_included_inner_instance.to_dict()
# create an instance of SubscriptionOfferCodesResponseIncludedInner from a dict
subscription_offer_codes_response_included_inner_from_dict = SubscriptionOfferCodesResponseIncludedInner.from_dict(subscription_offer_codes_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


