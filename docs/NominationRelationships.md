# NominationRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**related_apps** | [**InAppPurchaseRelationshipsApps**](InAppPurchaseRelationshipsApps.md) |  | [optional] 
**created_by_actor** | [**NominationRelationshipsCreatedByActor**](NominationRelationshipsCreatedByActor.md) |  | [optional] 
**last_modified_by_actor** | [**NominationRelationshipsCreatedByActor**](NominationRelationshipsCreatedByActor.md) |  | [optional] 
**submitted_by_actor** | [**NominationRelationshipsCreatedByActor**](NominationRelationshipsCreatedByActor.md) |  | [optional] 
**in_app_events** | [**NominationRelationshipsInAppEvents**](NominationRelationshipsInAppEvents.md) |  | [optional] 
**supported_territories** | [**NominationRelationshipsSupportedTerritories**](NominationRelationshipsSupportedTerritories.md) |  | [optional] 

## Example

```python
from openapi_client.models.nomination_relationships import NominationRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of NominationRelationships from a JSON string
nomination_relationships_instance = NominationRelationships.from_json(json)
# print the JSON string representation of the object
print(NominationRelationships.to_json())

# convert the object into a dict
nomination_relationships_dict = nomination_relationships_instance.to_dict()
# create an instance of NominationRelationships from a dict
nomination_relationships_from_dict = NominationRelationships.from_dict(nomination_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


