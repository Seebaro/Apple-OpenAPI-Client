# SubscriptionAppStoreReviewScreenshotResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionAppStoreReviewScreenshot**](SubscriptionAppStoreReviewScreenshot.md) |  | 
**included** | [**List[Subscription]**](Subscription.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_app_store_review_screenshot_response import SubscriptionAppStoreReviewScreenshotResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionAppStoreReviewScreenshotResponse from a JSON string
subscription_app_store_review_screenshot_response_instance = SubscriptionAppStoreReviewScreenshotResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionAppStoreReviewScreenshotResponse.to_json())

# convert the object into a dict
subscription_app_store_review_screenshot_response_dict = subscription_app_store_review_screenshot_response_instance.to_dict()
# create an instance of SubscriptionAppStoreReviewScreenshotResponse from a dict
subscription_app_store_review_screenshot_response_from_dict = SubscriptionAppStoreReviewScreenshotResponse.from_dict(subscription_app_store_review_screenshot_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


