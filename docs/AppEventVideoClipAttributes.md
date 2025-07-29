# AppEventVideoClipAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_size** | **int** |  | [optional] 
**file_name** | **str** |  | [optional] 
**preview_frame_time_code** | **str** |  | [optional] 
**video_url** | **str** |  | [optional] 
**preview_frame_image** | [**PreviewFrameImage**](PreviewFrameImage.md) |  | [optional] 
**preview_image** | [**ImageAsset**](ImageAsset.md) |  | [optional] 
**upload_operations** | [**List[UploadOperation]**](UploadOperation.md) |  | [optional] 
**asset_delivery_state** | [**AppMediaAssetState**](AppMediaAssetState.md) |  | [optional] 
**video_delivery_state** | [**AppMediaVideoState**](AppMediaVideoState.md) |  | [optional] 
**app_event_asset_type** | [**AppEventAssetType**](AppEventAssetType.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_video_clip_attributes import AppEventVideoClipAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventVideoClipAttributes from a JSON string
app_event_video_clip_attributes_instance = AppEventVideoClipAttributes.from_json(json)
# print the JSON string representation of the object
print(AppEventVideoClipAttributes.to_json())

# convert the object into a dict
app_event_video_clip_attributes_dict = app_event_video_clip_attributes_instance.to_dict()
# create an instance of AppEventVideoClipAttributes from a dict
app_event_video_clip_attributes_from_dict = AppEventVideoClipAttributes.from_dict(app_event_video_clip_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


