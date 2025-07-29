# AppClipAdvancedExperienceUpdateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**action** | [**AppClipAction**](AppClipAction.md) |  | [optional] 
**is_powered_by** | **bool** |  | [optional] 
**place** | [**AppClipAdvancedExperienceAttributesPlace**](AppClipAdvancedExperienceAttributesPlace.md) |  | [optional] 
**business_category** | **str** |  | [optional] 
**default_language** | [**AppClipAdvancedExperienceLanguage**](AppClipAdvancedExperienceLanguage.md) |  | [optional] 
**removed** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_advanced_experience_update_request_data_attributes import AppClipAdvancedExperienceUpdateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipAdvancedExperienceUpdateRequestDataAttributes from a JSON string
app_clip_advanced_experience_update_request_data_attributes_instance = AppClipAdvancedExperienceUpdateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(AppClipAdvancedExperienceUpdateRequestDataAttributes.to_json())

# convert the object into a dict
app_clip_advanced_experience_update_request_data_attributes_dict = app_clip_advanced_experience_update_request_data_attributes_instance.to_dict()
# create an instance of AppClipAdvancedExperienceUpdateRequestDataAttributes from a dict
app_clip_advanced_experience_update_request_data_attributes_from_dict = AppClipAdvancedExperienceUpdateRequestDataAttributes.from_dict(app_clip_advanced_experience_update_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


