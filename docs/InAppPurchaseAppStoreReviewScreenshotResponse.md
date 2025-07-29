# InAppPurchaseAppStoreReviewScreenshotResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**InAppPurchaseAppStoreReviewScreenshot**](InAppPurchaseAppStoreReviewScreenshot.md) |  | 
**included** | [**List[InAppPurchaseV2]**](InAppPurchaseV2.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_app_store_review_screenshot_response import InAppPurchaseAppStoreReviewScreenshotResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseAppStoreReviewScreenshotResponse from a JSON string
in_app_purchase_app_store_review_screenshot_response_instance = InAppPurchaseAppStoreReviewScreenshotResponse.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseAppStoreReviewScreenshotResponse.to_json())

# convert the object into a dict
in_app_purchase_app_store_review_screenshot_response_dict = in_app_purchase_app_store_review_screenshot_response_instance.to_dict()
# create an instance of InAppPurchaseAppStoreReviewScreenshotResponse from a dict
in_app_purchase_app_store_review_screenshot_response_from_dict = InAppPurchaseAppStoreReviewScreenshotResponse.from_dict(in_app_purchase_app_store_review_screenshot_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


