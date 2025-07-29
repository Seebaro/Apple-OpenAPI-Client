# AppClipAdvancedExperiencesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppClipAdvancedExperience]**](AppClipAdvancedExperience.md) |  | 
**included** | [**List[AppClipAdvancedExperiencesResponseIncludedInner]**](AppClipAdvancedExperiencesResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_advanced_experiences_response import AppClipAdvancedExperiencesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipAdvancedExperiencesResponse from a JSON string
app_clip_advanced_experiences_response_instance = AppClipAdvancedExperiencesResponse.from_json(json)
# print the JSON string representation of the object
print(AppClipAdvancedExperiencesResponse.to_json())

# convert the object into a dict
app_clip_advanced_experiences_response_dict = app_clip_advanced_experiences_response_instance.to_dict()
# create an instance of AppClipAdvancedExperiencesResponse from a dict
app_clip_advanced_experiences_response_from_dict = AppClipAdvancedExperiencesResponse.from_dict(app_clip_advanced_experiences_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


