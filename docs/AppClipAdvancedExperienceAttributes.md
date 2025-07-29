# AppClipAdvancedExperienceAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**link** | **str** |  | [optional] 
**version** | **int** |  | [optional] 
**status** | **str** |  | [optional] 
**action** | [**AppClipAction**](AppClipAction.md) |  | [optional] 
**is_powered_by** | **bool** |  | [optional] 
**place** | [**AppClipAdvancedExperienceAttributesPlace**](AppClipAdvancedExperienceAttributesPlace.md) |  | [optional] 
**place_status** | **str** |  | [optional] 
**business_category** | **str** |  | [optional] 
**default_language** | [**AppClipAdvancedExperienceLanguage**](AppClipAdvancedExperienceLanguage.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_advanced_experience_attributes import AppClipAdvancedExperienceAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipAdvancedExperienceAttributes from a JSON string
app_clip_advanced_experience_attributes_instance = AppClipAdvancedExperienceAttributes.from_json(json)
# print the JSON string representation of the object
print(AppClipAdvancedExperienceAttributes.to_json())

# convert the object into a dict
app_clip_advanced_experience_attributes_dict = app_clip_advanced_experience_attributes_instance.to_dict()
# create an instance of AppClipAdvancedExperienceAttributes from a dict
app_clip_advanced_experience_attributes_from_dict = AppClipAdvancedExperienceAttributes.from_dict(app_clip_advanced_experience_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


