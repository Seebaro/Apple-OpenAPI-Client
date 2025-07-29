# AppClipDefaultExperienceLocalizationCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppClipDefaultExperienceLocalizationCreateRequestDataAttributes**](AppClipDefaultExperienceLocalizationCreateRequestDataAttributes.md) |  | 
**relationships** | [**AppClipAppStoreReviewDetailCreateRequestDataRelationships**](AppClipAppStoreReviewDetailCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.app_clip_default_experience_localization_create_request_data import AppClipDefaultExperienceLocalizationCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipDefaultExperienceLocalizationCreateRequestData from a JSON string
app_clip_default_experience_localization_create_request_data_instance = AppClipDefaultExperienceLocalizationCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppClipDefaultExperienceLocalizationCreateRequestData.to_json())

# convert the object into a dict
app_clip_default_experience_localization_create_request_data_dict = app_clip_default_experience_localization_create_request_data_instance.to_dict()
# create an instance of AppClipDefaultExperienceLocalizationCreateRequestData from a dict
app_clip_default_experience_localization_create_request_data_from_dict = AppClipDefaultExperienceLocalizationCreateRequestData.from_dict(app_clip_default_experience_localization_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


