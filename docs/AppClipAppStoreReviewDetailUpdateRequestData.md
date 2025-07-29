# AppClipAppStoreReviewDetailUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipAppStoreReviewDetailAttributes**](AppClipAppStoreReviewDetailAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_app_store_review_detail_update_request_data import AppClipAppStoreReviewDetailUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipAppStoreReviewDetailUpdateRequestData from a JSON string
app_clip_app_store_review_detail_update_request_data_instance = AppClipAppStoreReviewDetailUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppClipAppStoreReviewDetailUpdateRequestData.to_json())

# convert the object into a dict
app_clip_app_store_review_detail_update_request_data_dict = app_clip_app_store_review_detail_update_request_data_instance.to_dict()
# create an instance of AppClipAppStoreReviewDetailUpdateRequestData from a dict
app_clip_app_store_review_detail_update_request_data_from_dict = AppClipAppStoreReviewDetailUpdateRequestData.from_dict(app_clip_app_store_review_detail_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


