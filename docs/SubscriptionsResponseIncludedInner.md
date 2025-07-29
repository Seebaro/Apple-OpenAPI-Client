# SubscriptionsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**InAppPurchaseImageAttributes**](InAppPurchaseImageAttributes.md) |  | [optional] 
**relationships** | [**SubscriptionAppStoreReviewScreenshotRelationships**](SubscriptionAppStoreReviewScreenshotRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscriptions_response_included_inner import SubscriptionsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionsResponseIncludedInner from a JSON string
subscriptions_response_included_inner_instance = SubscriptionsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(SubscriptionsResponseIncludedInner.to_json())

# convert the object into a dict
subscriptions_response_included_inner_dict = subscriptions_response_included_inner_instance.to_dict()
# create an instance of SubscriptionsResponseIncludedInner from a dict
subscriptions_response_included_inner_from_dict = SubscriptionsResponseIncludedInner.from_dict(subscriptions_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


