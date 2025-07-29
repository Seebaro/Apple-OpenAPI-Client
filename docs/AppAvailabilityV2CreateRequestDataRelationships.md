# AppAvailabilityV2CreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app** | [**AccessibilityDeclarationCreateRequestDataRelationshipsApp**](AccessibilityDeclarationCreateRequestDataRelationshipsApp.md) |  | 
**territory_availabilities** | [**AppAvailabilityV2CreateRequestDataRelationshipsTerritoryAvailabilities**](AppAvailabilityV2CreateRequestDataRelationshipsTerritoryAvailabilities.md) |  | 

## Example

```python
from openapi_client.models.app_availability_v2_create_request_data_relationships import AppAvailabilityV2CreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppAvailabilityV2CreateRequestDataRelationships from a JSON string
app_availability_v2_create_request_data_relationships_instance = AppAvailabilityV2CreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(AppAvailabilityV2CreateRequestDataRelationships.to_json())

# convert the object into a dict
app_availability_v2_create_request_data_relationships_dict = app_availability_v2_create_request_data_relationships_instance.to_dict()
# create an instance of AppAvailabilityV2CreateRequestDataRelationships from a dict
app_availability_v2_create_request_data_relationships_from_dict = AppAvailabilityV2CreateRequestDataRelationships.from_dict(app_availability_v2_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


