# AppEventLocalizationRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app_event** | [**AppEventLocalizationRelationshipsAppEvent**](AppEventLocalizationRelationshipsAppEvent.md) |  | [optional] 
**app_event_screenshots** | [**AppEventLocalizationRelationshipsAppEventScreenshots**](AppEventLocalizationRelationshipsAppEventScreenshots.md) |  | [optional] 
**app_event_video_clips** | [**AppEventLocalizationRelationshipsAppEventVideoClips**](AppEventLocalizationRelationshipsAppEventVideoClips.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_localization_relationships import AppEventLocalizationRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventLocalizationRelationships from a JSON string
app_event_localization_relationships_instance = AppEventLocalizationRelationships.from_json(json)
# print the JSON string representation of the object
print(AppEventLocalizationRelationships.to_json())

# convert the object into a dict
app_event_localization_relationships_dict = app_event_localization_relationships_instance.to_dict()
# create an instance of AppEventLocalizationRelationships from a dict
app_event_localization_relationships_from_dict = AppEventLocalizationRelationships.from_dict(app_event_localization_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


