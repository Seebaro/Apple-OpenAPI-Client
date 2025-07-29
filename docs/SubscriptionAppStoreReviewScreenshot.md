# SubscriptionAppStoreReviewScreenshot


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppScreenshotAttributes**](AppScreenshotAttributes.md) |  | [optional] 
**relationships** | [**SubscriptionAppStoreReviewScreenshotRelationships**](SubscriptionAppStoreReviewScreenshotRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_app_store_review_screenshot import SubscriptionAppStoreReviewScreenshot

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionAppStoreReviewScreenshot from a JSON string
subscription_app_store_review_screenshot_instance = SubscriptionAppStoreReviewScreenshot.from_json(json)
# print the JSON string representation of the object
print(SubscriptionAppStoreReviewScreenshot.to_json())

# convert the object into a dict
subscription_app_store_review_screenshot_dict = subscription_app_store_review_screenshot_instance.to_dict()
# create an instance of SubscriptionAppStoreReviewScreenshot from a dict
subscription_app_store_review_screenshot_from_dict = SubscriptionAppStoreReviewScreenshot.from_dict(subscription_app_store_review_screenshot_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


