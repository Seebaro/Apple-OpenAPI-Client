# AppClipAdvancedExperienceResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppClipAdvancedExperience**](AppClipAdvancedExperience.md) |  | 
**included** | [**List[AppClipAdvancedExperiencesResponseIncludedInner]**](AppClipAdvancedExperiencesResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_clip_advanced_experience_response import AppClipAdvancedExperienceResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipAdvancedExperienceResponse from a JSON string
app_clip_advanced_experience_response_instance = AppClipAdvancedExperienceResponse.from_json(json)
# print the JSON string representation of the object
print(AppClipAdvancedExperienceResponse.to_json())

# convert the object into a dict
app_clip_advanced_experience_response_dict = app_clip_advanced_experience_response_instance.to_dict()
# create an instance of AppClipAdvancedExperienceResponse from a dict
app_clip_advanced_experience_response_from_dict = AppClipAdvancedExperienceResponse.from_dict(app_clip_advanced_experience_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


