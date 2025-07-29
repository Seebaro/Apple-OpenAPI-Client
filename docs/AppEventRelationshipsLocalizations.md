# AppEventRelationshipsLocalizations


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppEventScreenshotRelationshipsAppEventLocalizationData]**](AppEventScreenshotRelationshipsAppEventLocalizationData.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_relationships_localizations import AppEventRelationshipsLocalizations

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventRelationshipsLocalizations from a JSON string
app_event_relationships_localizations_instance = AppEventRelationshipsLocalizations.from_json(json)
# print the JSON string representation of the object
print(AppEventRelationshipsLocalizations.to_json())

# convert the object into a dict
app_event_relationships_localizations_dict = app_event_relationships_localizations_instance.to_dict()
# create an instance of AppEventRelationshipsLocalizations from a dict
app_event_relationships_localizations_from_dict = AppEventRelationshipsLocalizations.from_dict(app_event_relationships_localizations_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


