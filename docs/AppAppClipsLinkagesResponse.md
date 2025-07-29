# AppAppClipsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppClipAdvancedExperienceRelationshipsAppClipData]**](AppClipAdvancedExperienceRelationshipsAppClipData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_app_clips_linkages_response import AppAppClipsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppAppClipsLinkagesResponse from a JSON string
app_app_clips_linkages_response_instance = AppAppClipsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppAppClipsLinkagesResponse.to_json())

# convert the object into a dict
app_app_clips_linkages_response_dict = app_app_clips_linkages_response_instance.to_dict()
# create an instance of AppAppClipsLinkagesResponse from a dict
app_app_clips_linkages_response_from_dict = AppAppClipsLinkagesResponse.from_dict(app_app_clips_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


