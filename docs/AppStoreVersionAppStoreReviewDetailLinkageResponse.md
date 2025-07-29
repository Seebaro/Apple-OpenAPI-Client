# AppStoreVersionAppStoreReviewDetailLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppStoreReviewAttachmentRelationshipsAppStoreReviewDetailData**](AppStoreReviewAttachmentRelationshipsAppStoreReviewDetailData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_app_store_review_detail_linkage_response import AppStoreVersionAppStoreReviewDetailLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionAppStoreReviewDetailLinkageResponse from a JSON string
app_store_version_app_store_review_detail_linkage_response_instance = AppStoreVersionAppStoreReviewDetailLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionAppStoreReviewDetailLinkageResponse.to_json())

# convert the object into a dict
app_store_version_app_store_review_detail_linkage_response_dict = app_store_version_app_store_review_detail_linkage_response_instance.to_dict()
# create an instance of AppStoreVersionAppStoreReviewDetailLinkageResponse from a dict
app_store_version_app_store_review_detail_linkage_response_from_dict = AppStoreVersionAppStoreReviewDetailLinkageResponse.from_dict(app_store_version_app_store_review_detail_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


