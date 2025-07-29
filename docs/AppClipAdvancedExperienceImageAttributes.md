# AppClipAdvancedExperienceImageAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_size** | **int** |  | [optional] 
**file_name** | **str** |  | [optional] 
**source_file_checksum** | **str** |  | [optional] 
**image_asset** | [**ImageAsset**](ImageAsset.md) |  | [optional] 
**upload_operations** | [**List[UploadOperation]**](UploadOperation.md) |  | [optional] 
**asset_delivery_state** | [**AppMediaAssetState**](AppMediaAssetState.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_advanced_experience_image_attributes import AppClipAdvancedExperienceImageAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipAdvancedExperienceImageAttributes from a JSON string
app_clip_advanced_experience_image_attributes_instance = AppClipAdvancedExperienceImageAttributes.from_json(json)
# print the JSON string representation of the object
print(AppClipAdvancedExperienceImageAttributes.to_json())

# convert the object into a dict
app_clip_advanced_experience_image_attributes_dict = app_clip_advanced_experience_image_attributes_instance.to_dict()
# create an instance of AppClipAdvancedExperienceImageAttributes from a dict
app_clip_advanced_experience_image_attributes_from_dict = AppClipAdvancedExperienceImageAttributes.from_dict(app_clip_advanced_experience_image_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


