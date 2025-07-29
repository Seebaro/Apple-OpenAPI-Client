# AppClipAppStoreReviewDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipAppStoreReviewDetailAttributes**](AppClipAppStoreReviewDetailAttributes.md) |  | [optional] 
**relationships** | [**AppClipAppStoreReviewDetailRelationships**](AppClipAppStoreReviewDetailRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_app_store_review_detail import AppClipAppStoreReviewDetail

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipAppStoreReviewDetail from a JSON string
app_clip_app_store_review_detail_instance = AppClipAppStoreReviewDetail.from_json(json)
# print the JSON string representation of the object
print(AppClipAppStoreReviewDetail.to_json())

# convert the object into a dict
app_clip_app_store_review_detail_dict = app_clip_app_store_review_detail_instance.to_dict()
# create an instance of AppClipAppStoreReviewDetail from a dict
app_clip_app_store_review_detail_from_dict = AppClipAppStoreReviewDetail.from_dict(app_clip_app_store_review_detail_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


