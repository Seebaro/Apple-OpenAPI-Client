# AppEventVideoClip


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppEventVideoClipAttributes**](AppEventVideoClipAttributes.md) |  | [optional] 
**relationships** | [**AppEventScreenshotRelationships**](AppEventScreenshotRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_video_clip import AppEventVideoClip

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventVideoClip from a JSON string
app_event_video_clip_instance = AppEventVideoClip.from_json(json)
# print the JSON string representation of the object
print(AppEventVideoClip.to_json())

# convert the object into a dict
app_event_video_clip_dict = app_event_video_clip_instance.to_dict()
# create an instance of AppEventVideoClip from a dict
app_event_video_clip_from_dict = AppEventVideoClip.from_dict(app_event_video_clip_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


