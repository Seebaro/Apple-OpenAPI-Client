# AppClipAdvancedExperienceImageUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipAdvancedExperienceImageUpdateRequestDataAttributes**](AppClipAdvancedExperienceImageUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_advanced_experience_image_update_request_data import AppClipAdvancedExperienceImageUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipAdvancedExperienceImageUpdateRequestData from a JSON string
app_clip_advanced_experience_image_update_request_data_instance = AppClipAdvancedExperienceImageUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppClipAdvancedExperienceImageUpdateRequestData.to_json())

# convert the object into a dict
app_clip_advanced_experience_image_update_request_data_dict = app_clip_advanced_experience_image_update_request_data_instance.to_dict()
# create an instance of AppClipAdvancedExperienceImageUpdateRequestData from a dict
app_clip_advanced_experience_image_update_request_data_from_dict = AppClipAdvancedExperienceImageUpdateRequestData.from_dict(app_clip_advanced_experience_image_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


