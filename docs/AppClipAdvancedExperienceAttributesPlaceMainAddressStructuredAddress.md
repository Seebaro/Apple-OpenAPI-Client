# AppClipAdvancedExperienceAttributesPlaceMainAddressStructuredAddress


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**street_address** | **List[str]** |  | [optional] 
**floor** | **str** |  | [optional] 
**neighborhood** | **str** |  | [optional] 
**locality** | **str** |  | [optional] 
**state_province** | **str** |  | [optional] 
**postal_code** | **str** |  | [optional] 
**country_code** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_advanced_experience_attributes_place_main_address_structured_address import AppClipAdvancedExperienceAttributesPlaceMainAddressStructuredAddress

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipAdvancedExperienceAttributesPlaceMainAddressStructuredAddress from a JSON string
app_clip_advanced_experience_attributes_place_main_address_structured_address_instance = AppClipAdvancedExperienceAttributesPlaceMainAddressStructuredAddress.from_json(json)
# print the JSON string representation of the object
print(AppClipAdvancedExperienceAttributesPlaceMainAddressStructuredAddress.to_json())

# convert the object into a dict
app_clip_advanced_experience_attributes_place_main_address_structured_address_dict = app_clip_advanced_experience_attributes_place_main_address_structured_address_instance.to_dict()
# create an instance of AppClipAdvancedExperienceAttributesPlaceMainAddressStructuredAddress from a dict
app_clip_advanced_experience_attributes_place_main_address_structured_address_from_dict = AppClipAdvancedExperienceAttributesPlaceMainAddressStructuredAddress.from_dict(app_clip_advanced_experience_attributes_place_main_address_structured_address_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


