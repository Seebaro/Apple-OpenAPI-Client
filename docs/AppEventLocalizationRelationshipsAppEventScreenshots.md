# AppEventLocalizationRelationshipsAppEventScreenshots


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppEventLocalizationRelationshipsAppEventScreenshotsDataInner]**](AppEventLocalizationRelationshipsAppEventScreenshotsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_localization_relationships_app_event_screenshots import AppEventLocalizationRelationshipsAppEventScreenshots

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventLocalizationRelationshipsAppEventScreenshots from a JSON string
app_event_localization_relationships_app_event_screenshots_instance = AppEventLocalizationRelationshipsAppEventScreenshots.from_json(json)
# print the JSON string representation of the object
print(AppEventLocalizationRelationshipsAppEventScreenshots.to_json())

# convert the object into a dict
app_event_localization_relationships_app_event_screenshots_dict = app_event_localization_relationships_app_event_screenshots_instance.to_dict()
# create an instance of AppEventLocalizationRelationshipsAppEventScreenshots from a dict
app_event_localization_relationships_app_event_screenshots_from_dict = AppEventLocalizationRelationshipsAppEventScreenshots.from_dict(app_event_localization_relationships_app_event_screenshots_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


