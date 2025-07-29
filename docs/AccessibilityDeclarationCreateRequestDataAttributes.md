# AccessibilityDeclarationCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**device_family** | [**DeviceFamily**](DeviceFamily.md) |  | 
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
from openapi_client.models.accessibility_declaration_create_request_data_attributes import AccessibilityDeclarationCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AccessibilityDeclarationCreateRequestDataAttributes from a JSON string
accessibility_declaration_create_request_data_attributes_instance = AccessibilityDeclarationCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(AccessibilityDeclarationCreateRequestDataAttributes.to_json())

# convert the object into a dict
accessibility_declaration_create_request_data_attributes_dict = accessibility_declaration_create_request_data_attributes_instance.to_dict()
# create an instance of AccessibilityDeclarationCreateRequestDataAttributes from a dict
accessibility_declaration_create_request_data_attributes_from_dict = AccessibilityDeclarationCreateRequestDataAttributes.from_dict(accessibility_declaration_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


