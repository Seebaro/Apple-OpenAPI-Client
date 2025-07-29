# AccessibilityDeclarationAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**device_family** | [**DeviceFamily**](DeviceFamily.md) |  | [optional] 
**state** | **str** |  | [optional] 
**supports_audio_descriptions** | **bool** |  | [optional] 
**supports_captions** | **bool** |  | [optional] 
**supports_dark_interface** | **bool** |  | [optional] 
**supports_differentiate_without_color_alone** | **bool** |  | [optional] 
**supports_larger_text** | **bool** |  | [optional] 
**supports_reduced_motion** | **bool** |  | [optional] 
**supports_sufficient_contrast** | **bool** |  | [optional] 
**supports_voice_control** | **bool** |  | [optional] 
**supports_voiceover** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.accessibility_declaration_attributes import AccessibilityDeclarationAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AccessibilityDeclarationAttributes from a JSON string
accessibility_declaration_attributes_instance = AccessibilityDeclarationAttributes.from_json(json)
# print the JSON string representation of the object
print(AccessibilityDeclarationAttributes.to_json())

# convert the object into a dict
accessibility_declaration_attributes_dict = accessibility_declaration_attributes_instance.to_dict()
# create an instance of AccessibilityDeclarationAttributes from a dict
accessibility_declaration_attributes_from_dict = AccessibilityDeclarationAttributes.from_dict(accessibility_declaration_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


