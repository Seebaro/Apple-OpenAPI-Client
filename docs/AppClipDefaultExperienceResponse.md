# AppClipDefaultExperienceResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppClipDefaultExperience**](AppClipDefaultExperience.md) |  | 
**included** | [**List[AppClipDefaultExperiencesResponseIncludedInner]**](AppClipDefaultExperiencesResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_clip_default_experience_response import AppClipDefaultExperienceResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipDefaultExperienceResponse from a JSON string
app_clip_default_experience_response_instance = AppClipDefaultExperienceResponse.from_json(json)
# print the JSON string representation of the object
print(AppClipDefaultExperienceResponse.to_json())

# convert the object into a dict
app_clip_default_experience_response_dict = app_clip_default_experience_response_instance.to_dict()
# create an instance of AppClipDefaultExperienceResponse from a dict
app_clip_default_experience_response_from_dict = AppClipDefaultExperienceResponse.from_dict(app_clip_default_experience_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


