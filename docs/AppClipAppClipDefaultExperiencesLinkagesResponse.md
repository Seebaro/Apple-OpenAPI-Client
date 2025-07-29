# AppClipAppClipDefaultExperiencesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppClipAppStoreReviewDetailRelationshipsAppClipDefaultExperienceData]**](AppClipAppStoreReviewDetailRelationshipsAppClipDefaultExperienceData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_app_clip_default_experiences_linkages_response import AppClipAppClipDefaultExperiencesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipAppClipDefaultExperiencesLinkagesResponse from a JSON string
app_clip_app_clip_default_experiences_linkages_response_instance = AppClipAppClipDefaultExperiencesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppClipAppClipDefaultExperiencesLinkagesResponse.to_json())

# convert the object into a dict
app_clip_app_clip_default_experiences_linkages_response_dict = app_clip_app_clip_default_experiences_linkages_response_instance.to_dict()
# create an instance of AppClipAppClipDefaultExperiencesLinkagesResponse from a dict
app_clip_app_clip_default_experiences_linkages_response_from_dict = AppClipAppClipDefaultExperiencesLinkagesResponse.from_dict(app_clip_app_clip_default_experiences_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


