# AppStoreReviewAttachment


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
from openapi_client.models.app_store_review_attachment import AppStoreReviewAttachment

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreReviewAttachment from a JSON string
app_store_review_attachment_instance = AppStoreReviewAttachment.from_json(json)
# print the JSON string representation of the object
print(AppStoreReviewAttachment.to_json())

# convert the object into a dict
app_store_review_attachment_dict = app_store_review_attachment_instance.to_dict()
# create an instance of AppStoreReviewAttachment from a dict
app_store_review_attachment_from_dict = AppStoreReviewAttachment.from_dict(app_store_review_attachment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


