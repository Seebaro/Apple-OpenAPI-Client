# SubscriptionAppStoreReviewScreenshotUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipAdvancedExperienceImageUpdateRequestDataAttributes**](AppClipAdvancedExperienceImageUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_app_store_review_screenshot_update_request_data import SubscriptionAppStoreReviewScreenshotUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionAppStoreReviewScreenshotUpdateRequestData from a JSON string
subscription_app_store_review_screenshot_update_request_data_instance = SubscriptionAppStoreReviewScreenshotUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionAppStoreReviewScreenshotUpdateRequestData.to_json())

# convert the object into a dict
subscription_app_store_review_screenshot_update_request_data_dict = subscription_app_store_review_screenshot_update_request_data_instance.to_dict()
# create an instance of SubscriptionAppStoreReviewScreenshotUpdateRequestData from a dict
subscription_app_store_review_screenshot_update_request_data_from_dict = SubscriptionAppStoreReviewScreenshotUpdateRequestData.from_dict(subscription_app_store_review_screenshot_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


