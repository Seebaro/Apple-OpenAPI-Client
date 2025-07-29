# AppClipDefaultExperienceLocalizationUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipDefaultExperienceLocalizationUpdateRequestDataAttributes**](AppClipDefaultExperienceLocalizationUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_default_experience_localization_update_request_data import AppClipDefaultExperienceLocalizationUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipDefaultExperienceLocalizationUpdateRequestData from a JSON string
app_clip_default_experience_localization_update_request_data_instance = AppClipDefaultExperienceLocalizationUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppClipDefaultExperienceLocalizationUpdateRequestData.to_json())

# convert the object into a dict
app_clip_default_experience_localization_update_request_data_dict = app_clip_default_experience_localization_update_request_data_instance.to_dict()
# create an instance of AppClipDefaultExperienceLocalizationUpdateRequestData from a dict
app_clip_default_experience_localization_update_request_data_from_dict = AppClipDefaultExperienceLocalizationUpdateRequestData.from_dict(app_clip_default_experience_localization_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


