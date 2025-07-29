# AppAvailabilityV2Relationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**territory_availabilities** | [**AppAvailabilityV2RelationshipsTerritoryAvailabilities**](AppAvailabilityV2RelationshipsTerritoryAvailabilities.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_availability_v2_relationships import AppAvailabilityV2Relationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppAvailabilityV2Relationships from a JSON string
app_availability_v2_relationships_instance = AppAvailabilityV2Relationships.from_json(json)
# print the JSON string representation of the object
print(AppAvailabilityV2Relationships.to_json())

# convert the object into a dict
app_availability_v2_relationships_dict = app_availability_v2_relationships_instance.to_dict()
# create an instance of AppAvailabilityV2Relationships from a dict
app_availability_v2_relationships_from_dict = AppAvailabilityV2Relationships.from_dict(app_availability_v2_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


