# AppClipAdvancedExperienceAttributesPlace


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**place_id** | **str** |  | [optional] 
**names** | **List[str]** |  | [optional] 
**main_address** | [**AppClipAdvancedExperienceAttributesPlaceMainAddress**](AppClipAdvancedExperienceAttributesPlaceMainAddress.md) |  | [optional] 
**display_point** | [**AppClipAdvancedExperienceAttributesPlaceDisplayPoint**](AppClipAdvancedExperienceAttributesPlaceDisplayPoint.md) |  | [optional] 
**map_action** | **str** |  | [optional] 
**relationship** | **str** |  | [optional] 
**phone_number** | [**AppClipAdvancedExperienceAttributesPlacePhoneNumber**](AppClipAdvancedExperienceAttributesPlacePhoneNumber.md) |  | [optional] 
**home_page** | **str** |  | [optional] 
**categories** | **List[str]** |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_advanced_experience_attributes_place import AppClipAdvancedExperienceAttributesPlace

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipAdvancedExperienceAttributesPlace from a JSON string
app_clip_advanced_experience_attributes_place_instance = AppClipAdvancedExperienceAttributesPlace.from_json(json)
# print the JSON string representation of the object
print(AppClipAdvancedExperienceAttributesPlace.to_json())

# convert the object into a dict
app_clip_advanced_experience_attributes_place_dict = app_clip_advanced_experience_attributes_place_instance.to_dict()
# create an instance of AppClipAdvancedExperienceAttributesPlace from a dict
app_clip_advanced_experience_attributes_place_from_dict = AppClipAdvancedExperienceAttributesPlace.from_dict(app_clip_advanced_experience_attributes_place_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


