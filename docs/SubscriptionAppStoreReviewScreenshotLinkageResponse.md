# SubscriptionAppStoreReviewScreenshotLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SubscriptionRelationshipsAppStoreReviewScreenshotData**](SubscriptionRelationshipsAppStoreReviewScreenshotData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.subscription_app_store_review_screenshot_linkage_response import SubscriptionAppStoreReviewScreenshotLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionAppStoreReviewScreenshotLinkageResponse from a JSON string
subscription_app_store_review_screenshot_linkage_response_instance = SubscriptionAppStoreReviewScreenshotLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionAppStoreReviewScreenshotLinkageResponse.to_json())

# convert the object into a dict
subscription_app_store_review_screenshot_linkage_response_dict = subscription_app_store_review_screenshot_linkage_response_instance.to_dict()
# create an instance of SubscriptionAppStoreReviewScreenshotLinkageResponse from a dict
subscription_app_store_review_screenshot_linkage_response_from_dict = SubscriptionAppStoreReviewScreenshotLinkageResponse.from_dict(subscription_app_store_review_screenshot_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


