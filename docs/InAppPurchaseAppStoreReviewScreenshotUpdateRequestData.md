# InAppPurchaseAppStoreReviewScreenshotUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipAdvancedExperienceImageUpdateRequestDataAttributes**](AppClipAdvancedExperienceImageUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_app_store_review_screenshot_update_request_data import InAppPurchaseAppStoreReviewScreenshotUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseAppStoreReviewScreenshotUpdateRequestData from a JSON string
in_app_purchase_app_store_review_screenshot_update_request_data_instance = InAppPurchaseAppStoreReviewScreenshotUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseAppStoreReviewScreenshotUpdateRequestData.to_json())

# convert the object into a dict
in_app_purchase_app_store_review_screenshot_update_request_data_dict = in_app_purchase_app_store_review_screenshot_update_request_data_instance.to_dict()
# create an instance of InAppPurchaseAppStoreReviewScreenshotUpdateRequestData from a dict
in_app_purchase_app_store_review_screenshot_update_request_data_from_dict = InAppPurchaseAppStoreReviewScreenshotUpdateRequestData.from_dict(in_app_purchase_app_store_review_screenshot_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


