# AppEventVideoClipUpdateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**preview_frame_time_code** | **str** |  | [optional] 
**uploaded** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.app_event_video_clip_update_request_data_attributes import AppEventVideoClipUpdateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventVideoClipUpdateRequestDataAttributes from a JSON string
app_event_video_clip_update_request_data_attributes_instance = AppEventVideoClipUpdateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(AppEventVideoClipUpdateRequestDataAttributes.to_json())

# convert the object into a dict
app_event_video_clip_update_request_data_attributes_dict = app_event_video_clip_update_request_data_attributes_instance.to_dict()
# create an instance of AppEventVideoClipUpdateRequestDataAttributes from a dict
app_event_video_clip_update_request_data_attributes_from_dict = AppEventVideoClipUpdateRequestDataAttributes.from_dict(app_event_video_clip_update_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


