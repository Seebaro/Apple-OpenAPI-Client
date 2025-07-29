# AppClipAdvancedExperiencesResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipAdvancedExperienceLocalizationAttributes**](AppClipAdvancedExperienceLocalizationAttributes.md) |  | [optional] 
**relationships** | [**AppClipRelationships**](AppClipRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_advanced_experiences_response_included_inner import AppClipAdvancedExperiencesResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipAdvancedExperiencesResponseIncludedInner from a JSON string
app_clip_advanced_experiences_response_included_inner_instance = AppClipAdvancedExperiencesResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppClipAdvancedExperiencesResponseIncludedInner.to_json())

# convert the object into a dict
app_clip_advanced_experiences_response_included_inner_dict = app_clip_advanced_experiences_response_included_inner_instance.to_dict()
# create an instance of AppClipAdvancedExperiencesResponseIncludedInner from a dict
app_clip_advanced_experiences_response_included_inner_from_dict = AppClipAdvancedExperiencesResponseIncludedInner.from_dict(app_clip_advanced_experiences_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


