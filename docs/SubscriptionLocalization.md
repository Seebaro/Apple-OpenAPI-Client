# SubscriptionLocalization


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**InAppPurchaseLocalizationAttributes**](InAppPurchaseLocalizationAttributes.md) |  | [optional] 
**relationships** | [**SubscriptionAppStoreReviewScreenshotRelationships**](SubscriptionAppStoreReviewScreenshotRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_localization import SubscriptionLocalization

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionLocalization from a JSON string
subscription_localization_instance = SubscriptionLocalization.from_json(json)
# print the JSON string representation of the object
print(SubscriptionLocalization.to_json())

# convert the object into a dict
subscription_localization_dict = subscription_localization_instance.to_dict()
# create an instance of SubscriptionLocalization from a dict
subscription_localization_from_dict = SubscriptionLocalization.from_dict(subscription_localization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


