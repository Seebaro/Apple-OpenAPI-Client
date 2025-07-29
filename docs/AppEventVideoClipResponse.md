# AppEventVideoClipResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppEventVideoClip**](AppEventVideoClip.md) |  | 
**included** | [**List[AppEventLocalization]**](AppEventLocalization.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_event_video_clip_response import AppEventVideoClipResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventVideoClipResponse from a JSON string
app_event_video_clip_response_instance = AppEventVideoClipResponse.from_json(json)
# print the JSON string representation of the object
print(AppEventVideoClipResponse.to_json())

# convert the object into a dict
app_event_video_clip_response_dict = app_event_video_clip_response_instance.to_dict()
# create an instance of AppEventVideoClipResponse from a dict
app_event_video_clip_response_from_dict = AppEventVideoClipResponse.from_dict(app_event_video_clip_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


