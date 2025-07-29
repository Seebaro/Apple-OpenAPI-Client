# SubscriptionAppStoreReviewScreenshotCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppClipAdvancedExperienceImageCreateRequestDataAttributes**](AppClipAdvancedExperienceImageCreateRequestDataAttributes.md) |  | 
**relationships** | [**SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationships**](SubscriptionAppStoreReviewScreenshotCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.subscription_app_store_review_screenshot_create_request_data import SubscriptionAppStoreReviewScreenshotCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionAppStoreReviewScreenshotCreateRequestData from a JSON string
subscription_app_store_review_screenshot_create_request_data_instance = SubscriptionAppStoreReviewScreenshotCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(SubscriptionAppStoreReviewScreenshotCreateRequestData.to_json())

# convert the object into a dict
subscription_app_store_review_screenshot_create_request_data_dict = subscription_app_store_review_screenshot_create_request_data_instance.to_dict()
# create an instance of SubscriptionAppStoreReviewScreenshotCreateRequestData from a dict
subscription_app_store_review_screenshot_create_request_data_from_dict = SubscriptionAppStoreReviewScreenshotCreateRequestData.from_dict(subscription_app_store_review_screenshot_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


