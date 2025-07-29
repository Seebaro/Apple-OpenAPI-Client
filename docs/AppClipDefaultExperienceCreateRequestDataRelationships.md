# AppClipDefaultExperienceCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app_clip** | [**AppClipAdvancedExperienceCreateRequestDataRelationshipsAppClip**](AppClipAdvancedExperienceCreateRequestDataRelationshipsAppClip.md) |  | 
**release_with_app_store_version** | [**AppClipDefaultExperienceCreateRequestDataRelationshipsReleaseWithAppStoreVersion**](AppClipDefaultExperienceCreateRequestDataRelationshipsReleaseWithAppStoreVersion.md) |  | [optional] 
**app_clip_default_experience_template** | [**AppClipAppStoreReviewDetailRelationshipsAppClipDefaultExperience**](AppClipAppStoreReviewDetailRelationshipsAppClipDefaultExperience.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_default_experience_create_request_data_relationships import AppClipDefaultExperienceCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipDefaultExperienceCreateRequestDataRelationships from a JSON string
app_clip_default_experience_create_request_data_relationships_instance = AppClipDefaultExperienceCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(AppClipDefaultExperienceCreateRequestDataRelationships.to_json())

# convert the object into a dict
app_clip_default_experience_create_request_data_relationships_dict = app_clip_default_experience_create_request_data_relationships_instance.to_dict()
# create an instance of AppClipDefaultExperienceCreateRequestDataRelationships from a dict
app_clip_default_experience_create_request_data_relationships_from_dict = AppClipDefaultExperienceCreateRequestDataRelationships.from_dict(app_clip_default_experience_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


