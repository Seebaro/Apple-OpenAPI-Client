# AppClipDefaultExperienceRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app_clip** | [**AppClipAdvancedExperienceRelationshipsAppClip**](AppClipAdvancedExperienceRelationshipsAppClip.md) |  | [optional] 
**release_with_app_store_version** | [**AppClipDefaultExperienceRelationshipsReleaseWithAppStoreVersion**](AppClipDefaultExperienceRelationshipsReleaseWithAppStoreVersion.md) |  | [optional] 
**app_clip_default_experience_localizations** | [**AppClipDefaultExperienceRelationshipsAppClipDefaultExperienceLocalizations**](AppClipDefaultExperienceRelationshipsAppClipDefaultExperienceLocalizations.md) |  | [optional] 
**app_clip_app_store_review_detail** | [**AppClipDefaultExperienceRelationshipsAppClipAppStoreReviewDetail**](AppClipDefaultExperienceRelationshipsAppClipAppStoreReviewDetail.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_default_experience_relationships import AppClipDefaultExperienceRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipDefaultExperienceRelationships from a JSON string
app_clip_default_experience_relationships_instance = AppClipDefaultExperienceRelationships.from_json(json)
# print the JSON string representation of the object
print(AppClipDefaultExperienceRelationships.to_json())

# convert the object into a dict
app_clip_default_experience_relationships_dict = app_clip_default_experience_relationships_instance.to_dict()
# create an instance of AppClipDefaultExperienceRelationships from a dict
app_clip_default_experience_relationships_from_dict = AppClipDefaultExperienceRelationships.from_dict(app_clip_default_experience_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


