# AppRelationshipsAppClips


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppClipAdvancedExperienceRelationshipsAppClipData]**](AppClipAdvancedExperienceRelationshipsAppClipData.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_relationships_app_clips import AppRelationshipsAppClips

# TODO update the JSON string below
json = "{}"
# create an instance of AppRelationshipsAppClips from a JSON string
app_relationships_app_clips_instance = AppRelationshipsAppClips.from_json(json)
# print the JSON string representation of the object
print(AppRelationshipsAppClips.to_json())

# convert the object into a dict
app_relationships_app_clips_dict = app_relationships_app_clips_instance.to_dict()
# create an instance of AppRelationshipsAppClips from a dict
app_relationships_app_clips_from_dict = AppRelationshipsAppClips.from_dict(app_relationships_app_clips_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


