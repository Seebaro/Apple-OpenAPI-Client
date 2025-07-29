# InAppPurchaseAppStoreReviewScreenshotCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppClipAdvancedExperienceImageCreateRequestDataAttributes**](AppClipAdvancedExperienceImageCreateRequestDataAttributes.md) |  | 
**relationships** | [**InAppPurchaseAppStoreReviewScreenshotCreateRequestDataRelationships**](InAppPurchaseAppStoreReviewScreenshotCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_app_store_review_screenshot_create_request_data import InAppPurchaseAppStoreReviewScreenshotCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseAppStoreReviewScreenshotCreateRequestData from a JSON string
in_app_purchase_app_store_review_screenshot_create_request_data_instance = InAppPurchaseAppStoreReviewScreenshotCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseAppStoreReviewScreenshotCreateRequestData.to_json())

# convert the object into a dict
in_app_purchase_app_store_review_screenshot_create_request_data_dict = in_app_purchase_app_store_review_screenshot_create_request_data_instance.to_dict()
# create an instance of InAppPurchaseAppStoreReviewScreenshotCreateRequestData from a dict
in_app_purchase_app_store_review_screenshot_create_request_data_from_dict = InAppPurchaseAppStoreReviewScreenshotCreateRequestData.from_dict(in_app_purchase_app_store_review_screenshot_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


