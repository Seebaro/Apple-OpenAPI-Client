# NominationRelationshipsInAppEvents


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppEventLocalizationRelationshipsAppEventData]**](AppEventLocalizationRelationshipsAppEventData.md) |  | [optional] 

## Example

```python
from openapi_client.models.nomination_relationships_in_app_events import NominationRelationshipsInAppEvents

# TODO update the JSON string below
json = "{}"
# create an instance of NominationRelationshipsInAppEvents from a JSON string
nomination_relationships_in_app_events_instance = NominationRelationshipsInAppEvents.from_json(json)
# print the JSON string representation of the object
print(NominationRelationshipsInAppEvents.to_json())

# convert the object into a dict
nomination_relationships_in_app_events_dict = nomination_relationships_in_app_events_instance.to_dict()
# create an instance of NominationRelationshipsInAppEvents from a dict
nomination_relationships_in_app_events_from_dict = NominationRelationshipsInAppEvents.from_dict(nomination_relationships_in_app_events_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


