# SubscriptionImage


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
from openapi_client.models.subscription_image import SubscriptionImage

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionImage from a JSON string
subscription_image_instance = SubscriptionImage.from_json(json)
# print the JSON string representation of the object
print(SubscriptionImage.to_json())

# convert the object into a dict
subscription_image_dict = subscription_image_instance.to_dict()
# create an instance of SubscriptionImage from a dict
subscription_image_from_dict = SubscriptionImage.from_dict(subscription_image_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


