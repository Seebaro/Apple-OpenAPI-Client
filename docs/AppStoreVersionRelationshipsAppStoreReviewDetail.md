# AppStoreVersionRelationshipsAppStoreReviewDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**data** | [**AppStoreReviewAttachmentRelationshipsAppStoreReviewDetailData**](AppStoreReviewAttachmentRelationshipsAppStoreReviewDetailData.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_relationships_app_store_review_detail import AppStoreVersionRelationshipsAppStoreReviewDetail

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionRelationshipsAppStoreReviewDetail from a JSON string
app_store_version_relationships_app_store_review_detail_instance = AppStoreVersionRelationshipsAppStoreReviewDetail.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionRelationshipsAppStoreReviewDetail.to_json())

# convert the object into a dict
app_store_version_relationships_app_store_review_detail_dict = app_store_version_relationships_app_store_review_detail_instance.to_dict()
# create an instance of AppStoreVersionRelationshipsAppStoreReviewDetail from a dict
app_store_version_relationships_app_store_review_detail_from_dict = AppStoreVersionRelationshipsAppStoreReviewDetail.from_dict(app_store_version_relationships_app_store_review_detail_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


