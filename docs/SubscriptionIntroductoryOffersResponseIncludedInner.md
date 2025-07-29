# SubscriptionIntroductoryOffersResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SubscriptionPricePointAttributes**](SubscriptionPricePointAttributes.md) |  | [optional] 
**relationships** | [**InAppPurchasePricePointRelationships**](InAppPurchasePricePointRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_introductory_offers_response_included_inner import SubscriptionIntroductoryOffersResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionIntroductoryOffersResponseIncludedInner from a JSON string
subscription_introductory_offers_response_included_inner_instance = SubscriptionIntroductoryOffersResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(SubscriptionIntroductoryOffersResponseIncludedInner.to_json())

# convert the object into a dict
subscription_introductory_offers_response_included_inner_dict = subscription_introductory_offers_response_included_inner_instance.to_dict()
# create an instance of SubscriptionIntroductoryOffersResponseIncludedInner from a dict
subscription_introductory_offers_response_included_inner_from_dict = SubscriptionIntroductoryOffersResponseIncludedInner.from_dict(subscription_introductory_offers_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


