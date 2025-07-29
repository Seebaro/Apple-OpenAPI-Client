# AppClipAdvancedExperienceCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**link** | **str** |  | 
**action** | [**AppClipAction**](AppClipAction.md) |  | [optional] 
**is_powered_by** | **bool** |  | 
**place** | [**AppClipAdvancedExperienceAttributesPlace**](AppClipAdvancedExperienceAttributesPlace.md) |  | [optional] 
**business_category** | **str** |  | [optional] 
**default_language** | [**AppClipAdvancedExperienceLanguage**](AppClipAdvancedExperienceLanguage.md) |  | 

## Example

```python
from openapi_client.models.app_clip_advanced_experience_create_request_data_attributes import AppClipAdvancedExperienceCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipAdvancedExperienceCreateRequestDataAttributes from a JSON string
app_clip_advanced_experience_create_request_data_attributes_instance = AppClipAdvancedExperienceCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(AppClipAdvancedExperienceCreateRequestDataAttributes.to_json())

# convert the object into a dict
app_clip_advanced_experience_create_request_data_attributes_dict = app_clip_advanced_experience_create_request_data_attributes_instance.to_dict()
# create an instance of AppClipAdvancedExperienceCreateRequestDataAttributes from a dict
app_clip_advanced_experience_create_request_data_attributes_from_dict = AppClipAdvancedExperienceCreateRequestDataAttributes.from_dict(app_clip_advanced_experience_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


