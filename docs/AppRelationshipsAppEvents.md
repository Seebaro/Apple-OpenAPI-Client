# AppRelationshipsAppEvents


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppEventLocalizationRelationshipsAppEventData]**](AppEventLocalizationRelationshipsAppEventData.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_relationships_app_events import AppRelationshipsAppEvents

# TODO update the JSON string below
json = "{}"
# create an instance of AppRelationshipsAppEvents from a JSON string
app_relationships_app_events_instance = AppRelationshipsAppEvents.from_json(json)
# print the JSON string representation of the object
print(AppRelationshipsAppEvents.to_json())

# convert the object into a dict
app_relationships_app_events_dict = app_relationships_app_events_instance.to_dict()
# create an instance of AppRelationshipsAppEvents from a dict
app_relationships_app_events_from_dict = AppRelationshipsAppEvents.from_dict(app_relationships_app_events_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


