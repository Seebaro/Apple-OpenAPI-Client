# AppStoreReviewDetailResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppStoreReviewAttachmentAttributes**](AppStoreReviewAttachmentAttributes.md) |  | [optional] 
**relationships** | [**AppStoreReviewAttachmentRelationships**](AppStoreReviewAttachmentRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_review_detail_response_included_inner import AppStoreReviewDetailResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreReviewDetailResponseIncludedInner from a JSON string
app_store_review_detail_response_included_inner_instance = AppStoreReviewDetailResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppStoreReviewDetailResponseIncludedInner.to_json())

# convert the object into a dict
app_store_review_detail_response_included_inner_dict = app_store_review_detail_response_included_inner_instance.to_dict()
# create an instance of AppStoreReviewDetailResponseIncludedInner from a dict
app_store_review_detail_response_included_inner_from_dict = AppStoreReviewDetailResponseIncludedInner.from_dict(app_store_review_detail_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


