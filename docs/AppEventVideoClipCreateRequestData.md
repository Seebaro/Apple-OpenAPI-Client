# AppEventVideoClipCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppEventVideoClipCreateRequestDataAttributes**](AppEventVideoClipCreateRequestDataAttributes.md) |  | 
**relationships** | [**AppEventScreenshotCreateRequestDataRelationships**](AppEventScreenshotCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.app_event_video_clip_create_request_data import AppEventVideoClipCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventVideoClipCreateRequestData from a JSON string
app_event_video_clip_create_request_data_instance = AppEventVideoClipCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppEventVideoClipCreateRequestData.to_json())

# convert the object into a dict
app_event_video_clip_create_request_data_dict = app_event_video_clip_create_request_data_instance.to_dict()
# create an instance of AppEventVideoClipCreateRequestData from a dict
app_event_video_clip_create_request_data_from_dict = AppEventVideoClipCreateRequestData.from_dict(app_event_video_clip_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


