# AppEventVideoClipUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppEventVideoClipUpdateRequestData**](AppEventVideoClipUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.app_event_video_clip_update_request import AppEventVideoClipUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventVideoClipUpdateRequest from a JSON string
app_event_video_clip_update_request_instance = AppEventVideoClipUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(AppEventVideoClipUpdateRequest.to_json())

# convert the object into a dict
app_event_video_clip_update_request_dict = app_event_video_clip_update_request_instance.to_dict()
# create an instance of AppEventVideoClipUpdateRequest from a dict
app_event_video_clip_update_request_from_dict = AppEventVideoClipUpdateRequest.from_dict(app_event_video_clip_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


