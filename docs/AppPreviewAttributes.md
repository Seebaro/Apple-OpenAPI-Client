# AppPreviewAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_size** | **int** |  | [optional] 
**file_name** | **str** |  | [optional] 
**source_file_checksum** | **str** |  | [optional] 
**preview_frame_time_code** | **str** |  | [optional] 
**mime_type** | **str** |  | [optional] 
**video_url** | **str** |  | [optional] 
**preview_frame_image** | [**PreviewFrameImage**](PreviewFrameImage.md) |  | [optional] 
**preview_image** | [**ImageAsset**](ImageAsset.md) |  | [optional] 
**upload_operations** | [**List[UploadOperation]**](UploadOperation.md) |  | [optional] 
**asset_delivery_state** | [**AppMediaAssetState**](AppMediaAssetState.md) |  | [optional] 
**video_delivery_state** | [**AppMediaVideoState**](AppMediaVideoState.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_preview_attributes import AppPreviewAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppPreviewAttributes from a JSON string
app_preview_attributes_instance = AppPreviewAttributes.from_json(json)
# print the JSON string representation of the object
print(AppPreviewAttributes.to_json())

# convert the object into a dict
app_preview_attributes_dict = app_preview_attributes_instance.to_dict()
# create an instance of AppPreviewAttributes from a dict
app_preview_attributes_from_dict = AppPreviewAttributes.from_dict(app_preview_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


