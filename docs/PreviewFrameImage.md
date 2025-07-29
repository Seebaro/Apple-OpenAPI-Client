# PreviewFrameImage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**image** | [**ImageAsset**](ImageAsset.md) |  | [optional] 
**state** | [**AppMediaPreviewFrameImageState**](AppMediaPreviewFrameImageState.md) |  | [optional] 

## Example

```python
from openapi_client.models.preview_frame_image import PreviewFrameImage

# TODO update the JSON string below
json = "{}"
# create an instance of PreviewFrameImage from a JSON string
preview_frame_image_instance = PreviewFrameImage.from_json(json)
# print the JSON string representation of the object
print(PreviewFrameImage.to_json())

# convert the object into a dict
preview_frame_image_dict = preview_frame_image_instance.to_dict()
# create an instance of PreviewFrameImage from a dict
preview_frame_image_from_dict = PreviewFrameImage.from_dict(preview_frame_image_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


