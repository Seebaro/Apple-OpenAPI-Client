# AppEventVideoClipCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_size** | **int** |  | 
**file_name** | **str** |  | 
**preview_frame_time_code** | **str** |  | [optional] 
**app_event_asset_type** | [**AppEventAssetType**](AppEventAssetType.md) |  | 

## Example

```python
from openapi_client.models.app_event_video_clip_create_request_data_attributes import AppEventVideoClipCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventVideoClipCreateRequestDataAttributes from a JSON string
app_event_video_clip_create_request_data_attributes_instance = AppEventVideoClipCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(AppEventVideoClipCreateRequestDataAttributes.to_json())

# convert the object into a dict
app_event_video_clip_create_request_data_attributes_dict = app_event_video_clip_create_request_data_attributes_instance.to_dict()
# create an instance of AppEventVideoClipCreateRequestDataAttributes from a dict
app_event_video_clip_create_request_data_attributes_from_dict = AppEventVideoClipCreateRequestDataAttributes.from_dict(app_event_video_clip_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


