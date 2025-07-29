# AppEventVideoClipCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppEventVideoClipCreateRequestData**](AppEventVideoClipCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.app_event_video_clip_create_request import AppEventVideoClipCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventVideoClipCreateRequest from a JSON string
app_event_video_clip_create_request_instance = AppEventVideoClipCreateRequest.from_json(json)
# print the JSON string representation of the object
print(AppEventVideoClipCreateRequest.to_json())

# convert the object into a dict
app_event_video_clip_create_request_dict = app_event_video_clip_create_request_instance.to_dict()
# create an instance of AppEventVideoClipCreateRequest from a dict
app_event_video_clip_create_request_from_dict = AppEventVideoClipCreateRequest.from_dict(app_event_video_clip_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


