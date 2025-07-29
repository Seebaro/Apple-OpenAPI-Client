# AppMediaPreviewFrameImageState


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**errors** | [**List[AppMediaStateError]**](AppMediaStateError.md) |  | [optional] 
**warnings** | [**List[AppMediaStateError]**](AppMediaStateError.md) |  | [optional] 
**state** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.app_media_preview_frame_image_state import AppMediaPreviewFrameImageState

# TODO update the JSON string below
json = "{}"
# create an instance of AppMediaPreviewFrameImageState from a JSON string
app_media_preview_frame_image_state_instance = AppMediaPreviewFrameImageState.from_json(json)
# print the JSON string representation of the object
print(AppMediaPreviewFrameImageState.to_json())

# convert the object into a dict
app_media_preview_frame_image_state_dict = app_media_preview_frame_image_state_instance.to_dict()
# create an instance of AppMediaPreviewFrameImageState from a dict
app_media_preview_frame_image_state_from_dict = AppMediaPreviewFrameImageState.from_dict(app_media_preview_frame_image_state_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


