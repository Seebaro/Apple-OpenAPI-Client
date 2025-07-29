# AppEventVideoClipsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppEventVideoClip]**](AppEventVideoClip.md) |  | 
**included** | [**List[AppEventLocalization]**](AppEventLocalization.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_video_clips_response import AppEventVideoClipsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventVideoClipsResponse from a JSON string
app_event_video_clips_response_instance = AppEventVideoClipsResponse.from_json(json)
# print the JSON string representation of the object
print(AppEventVideoClipsResponse.to_json())

# convert the object into a dict
app_event_video_clips_response_dict = app_event_video_clips_response_instance.to_dict()
# create an instance of AppEventVideoClipsResponse from a dict
app_event_video_clips_response_from_dict = AppEventVideoClipsResponse.from_dict(app_event_video_clips_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


