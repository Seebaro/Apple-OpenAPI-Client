# AppClipDefaultExperienceLocalization


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipDefaultExperienceLocalizationAttributes**](AppClipDefaultExperienceLocalizationAttributes.md) |  | [optional] 
**relationships** | [**AppClipDefaultExperienceLocalizationRelationships**](AppClipDefaultExperienceLocalizationRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_default_experience_localization import AppClipDefaultExperienceLocalization

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipDefaultExperienceLocalization from a JSON string
app_clip_default_experience_localization_instance = AppClipDefaultExperienceLocalization.from_json(json)
# print the JSON string representation of the object
print(AppClipDefaultExperienceLocalization.to_json())

# convert the object into a dict
app_clip_default_experience_localization_dict = app_clip_default_experience_localization_instance.to_dict()
# create an instance of AppClipDefaultExperienceLocalization from a dict
app_clip_default_experience_localization_from_dict = AppClipDefaultExperienceLocalization.from_dict(app_clip_default_experience_localization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


