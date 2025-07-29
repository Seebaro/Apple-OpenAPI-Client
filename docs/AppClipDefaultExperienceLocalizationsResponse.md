# AppClipDefaultExperienceLocalizationsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppClipDefaultExperienceLocalization]**](AppClipDefaultExperienceLocalization.md) |  | 
**included** | [**List[AppClipDefaultExperienceLocalizationsResponseIncludedInner]**](AppClipDefaultExperienceLocalizationsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_default_experience_localizations_response import AppClipDefaultExperienceLocalizationsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipDefaultExperienceLocalizationsResponse from a JSON string
app_clip_default_experience_localizations_response_instance = AppClipDefaultExperienceLocalizationsResponse.from_json(json)
# print the JSON string representation of the object
print(AppClipDefaultExperienceLocalizationsResponse.to_json())

# convert the object into a dict
app_clip_default_experience_localizations_response_dict = app_clip_default_experience_localizations_response_instance.to_dict()
# create an instance of AppClipDefaultExperienceLocalizationsResponse from a dict
app_clip_default_experience_localizations_response_from_dict = AppClipDefaultExperienceLocalizationsResponse.from_dict(app_clip_default_experience_localizations_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


