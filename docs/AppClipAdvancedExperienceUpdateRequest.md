# AppClipAdvancedExperienceUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppClipAdvancedExperienceUpdateRequestData**](AppClipAdvancedExperienceUpdateRequestData.md) |  | 
**included** | [**List[AppClipAdvancedExperienceLocalizationInlineCreate]**](AppClipAdvancedExperienceLocalizationInlineCreate.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_advanced_experience_update_request import AppClipAdvancedExperienceUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipAdvancedExperienceUpdateRequest from a JSON string
app_clip_advanced_experience_update_request_instance = AppClipAdvancedExperienceUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(AppClipAdvancedExperienceUpdateRequest.to_json())

# convert the object into a dict
app_clip_advanced_experience_update_request_dict = app_clip_advanced_experience_update_request_instance.to_dict()
# create an instance of AppClipAdvancedExperienceUpdateRequest from a dict
app_clip_advanced_experience_update_request_from_dict = AppClipAdvancedExperienceUpdateRequest.from_dict(app_clip_advanced_experience_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


