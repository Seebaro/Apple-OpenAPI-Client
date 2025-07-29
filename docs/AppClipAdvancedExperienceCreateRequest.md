# AppClipAdvancedExperienceCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppClipAdvancedExperienceCreateRequestData**](AppClipAdvancedExperienceCreateRequestData.md) |  | 
**included** | [**List[AppClipAdvancedExperienceLocalizationInlineCreate]**](AppClipAdvancedExperienceLocalizationInlineCreate.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_advanced_experience_create_request import AppClipAdvancedExperienceCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipAdvancedExperienceCreateRequest from a JSON string
app_clip_advanced_experience_create_request_instance = AppClipAdvancedExperienceCreateRequest.from_json(json)
# print the JSON string representation of the object
print(AppClipAdvancedExperienceCreateRequest.to_json())

# convert the object into a dict
app_clip_advanced_experience_create_request_dict = app_clip_advanced_experience_create_request_instance.to_dict()
# create an instance of AppClipAdvancedExperienceCreateRequest from a dict
app_clip_advanced_experience_create_request_from_dict = AppClipAdvancedExperienceCreateRequest.from_dict(app_clip_advanced_experience_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


