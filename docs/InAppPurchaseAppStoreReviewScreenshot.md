# InAppPurchaseAppStoreReviewScreenshot


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppScreenshotAttributes**](AppScreenshotAttributes.md) |  | [optional] 
**relationships** | [**InAppPurchaseAppStoreReviewScreenshotRelationships**](InAppPurchaseAppStoreReviewScreenshotRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_app_store_review_screenshot import InAppPurchaseAppStoreReviewScreenshot

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseAppStoreReviewScreenshot from a JSON string
in_app_purchase_app_store_review_screenshot_instance = InAppPurchaseAppStoreReviewScreenshot.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseAppStoreReviewScreenshot.to_json())

# convert the object into a dict
in_app_purchase_app_store_review_screenshot_dict = in_app_purchase_app_store_review_screenshot_instance.to_dict()
# create an instance of InAppPurchaseAppStoreReviewScreenshot from a dict
in_app_purchase_app_store_review_screenshot_from_dict = InAppPurchaseAppStoreReviewScreenshot.from_dict(in_app_purchase_app_store_review_screenshot_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


