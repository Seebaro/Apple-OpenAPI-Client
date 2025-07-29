# AppClipAdvancedExperienceUpdateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app_clip** | [**AppClipAdvancedExperienceRelationshipsAppClip**](AppClipAdvancedExperienceRelationshipsAppClip.md) |  | [optional] 
**header_image** | [**AppClipAdvancedExperienceRelationshipsHeaderImage**](AppClipAdvancedExperienceRelationshipsHeaderImage.md) |  | [optional] 
**localizations** | [**AppClipAdvancedExperienceUpdateRequestDataRelationshipsLocalizations**](AppClipAdvancedExperienceUpdateRequestDataRelationshipsLocalizations.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_advanced_experience_update_request_data_relationships import AppClipAdvancedExperienceUpdateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipAdvancedExperienceUpdateRequestDataRelationships from a JSON string
app_clip_advanced_experience_update_request_data_relationships_instance = AppClipAdvancedExperienceUpdateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(AppClipAdvancedExperienceUpdateRequestDataRelationships.to_json())

# convert the object into a dict
app_clip_advanced_experience_update_request_data_relationships_dict = app_clip_advanced_experience_update_request_data_relationships_instance.to_dict()
# create an instance of AppClipAdvancedExperienceUpdateRequestDataRelationships from a dict
app_clip_advanced_experience_update_request_data_relationships_from_dict = AppClipAdvancedExperienceUpdateRequestDataRelationships.from_dict(app_clip_advanced_experience_update_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


