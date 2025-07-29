# AppAvailabilityV2RelationshipsTerritoryAvailabilities


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppAvailabilityV2RelationshipsTerritoryAvailabilitiesDataInner]**](AppAvailabilityV2RelationshipsTerritoryAvailabilitiesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_availability_v2_relationships_territory_availabilities import AppAvailabilityV2RelationshipsTerritoryAvailabilities

# TODO update the JSON string below
json = "{}"
# create an instance of AppAvailabilityV2RelationshipsTerritoryAvailabilities from a JSON string
app_availability_v2_relationships_territory_availabilities_instance = AppAvailabilityV2RelationshipsTerritoryAvailabilities.from_json(json)
# print the JSON string representation of the object
print(AppAvailabilityV2RelationshipsTerritoryAvailabilities.to_json())

# convert the object into a dict
app_availability_v2_relationships_territory_availabilities_dict = app_availability_v2_relationships_territory_availabilities_instance.to_dict()
# create an instance of AppAvailabilityV2RelationshipsTerritoryAvailabilities from a dict
app_availability_v2_relationships_territory_availabilities_from_dict = AppAvailabilityV2RelationshipsTerritoryAvailabilities.from_dict(app_availability_v2_relationships_territory_availabilities_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


