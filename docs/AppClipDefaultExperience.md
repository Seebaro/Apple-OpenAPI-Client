# AppClipDefaultExperience


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipDefaultExperienceAttributes**](AppClipDefaultExperienceAttributes.md) |  | [optional] 
**relationships** | [**AppClipDefaultExperienceRelationships**](AppClipDefaultExperienceRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_default_experience import AppClipDefaultExperience

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipDefaultExperience from a JSON string
app_clip_default_experience_instance = AppClipDefaultExperience.from_json(json)
# print the JSON string representation of the object
print(AppClipDefaultExperience.to_json())

# convert the object into a dict
app_clip_default_experience_dict = app_clip_default_experience_instance.to_dict()
# create an instance of AppClipDefaultExperience from a dict
app_clip_default_experience_from_dict = AppClipDefaultExperience.from_dict(app_clip_default_experience_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


