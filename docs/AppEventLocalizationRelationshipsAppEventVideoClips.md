# AppEventLocalizationRelationshipsAppEventVideoClips


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppEventLocalizationRelationshipsAppEventVideoClipsDataInner]**](AppEventLocalizationRelationshipsAppEventVideoClipsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_localization_relationships_app_event_video_clips import AppEventLocalizationRelationshipsAppEventVideoClips

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventLocalizationRelationshipsAppEventVideoClips from a JSON string
app_event_localization_relationships_app_event_video_clips_instance = AppEventLocalizationRelationshipsAppEventVideoClips.from_json(json)
# print the JSON string representation of the object
print(AppEventLocalizationRelationshipsAppEventVideoClips.to_json())

# convert the object into a dict
app_event_localization_relationships_app_event_video_clips_dict = app_event_localization_relationships_app_event_video_clips_instance.to_dict()
# create an instance of AppEventLocalizationRelationshipsAppEventVideoClips from a dict
app_event_localization_relationships_app_event_video_clips_from_dict = AppEventLocalizationRelationshipsAppEventVideoClips.from_dict(app_event_localization_relationships_app_event_video_clips_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


