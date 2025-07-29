# AppEventLocalizationAppEventVideoClipsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppEventLocalizationRelationshipsAppEventVideoClipsDataInner]**](AppEventLocalizationRelationshipsAppEventVideoClipsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_localization_app_event_video_clips_linkages_response import AppEventLocalizationAppEventVideoClipsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventLocalizationAppEventVideoClipsLinkagesResponse from a JSON string
app_event_localization_app_event_video_clips_linkages_response_instance = AppEventLocalizationAppEventVideoClipsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppEventLocalizationAppEventVideoClipsLinkagesResponse.to_json())

# convert the object into a dict
app_event_localization_app_event_video_clips_linkages_response_dict = app_event_localization_app_event_video_clips_linkages_response_instance.to_dict()
# create an instance of AppEventLocalizationAppEventVideoClipsLinkagesResponse from a dict
app_event_localization_app_event_video_clips_linkages_response_from_dict = AppEventLocalizationAppEventVideoClipsLinkagesResponse.from_dict(app_event_localization_app_event_video_clips_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


