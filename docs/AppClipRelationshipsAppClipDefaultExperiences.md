# AppClipRelationshipsAppClipDefaultExperiences


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppClipAppStoreReviewDetailRelationshipsAppClipDefaultExperienceData]**](AppClipAppStoreReviewDetailRelationshipsAppClipDefaultExperienceData.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_relationships_app_clip_default_experiences import AppClipRelationshipsAppClipDefaultExperiences

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipRelationshipsAppClipDefaultExperiences from a JSON string
app_clip_relationships_app_clip_default_experiences_instance = AppClipRelationshipsAppClipDefaultExperiences.from_json(json)
# print the JSON string representation of the object
print(AppClipRelationshipsAppClipDefaultExperiences.to_json())

# convert the object into a dict
app_clip_relationships_app_clip_default_experiences_dict = app_clip_relationships_app_clip_default_experiences_instance.to_dict()
# create an instance of AppClipRelationshipsAppClipDefaultExperiences from a dict
app_clip_relationships_app_clip_default_experiences_from_dict = AppClipRelationshipsAppClipDefaultExperiences.from_dict(app_clip_relationships_app_clip_default_experiences_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


