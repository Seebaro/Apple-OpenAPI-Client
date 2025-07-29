# AppAvailabilityV2TerritoryAvailabilitiesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppAvailabilityV2RelationshipsTerritoryAvailabilitiesDataInner]**](AppAvailabilityV2RelationshipsTerritoryAvailabilitiesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_availability_v2_territory_availabilities_linkages_response import AppAvailabilityV2TerritoryAvailabilitiesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppAvailabilityV2TerritoryAvailabilitiesLinkagesResponse from a JSON string
app_availability_v2_territory_availabilities_linkages_response_instance = AppAvailabilityV2TerritoryAvailabilitiesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppAvailabilityV2TerritoryAvailabilitiesLinkagesResponse.to_json())

# convert the object into a dict
app_availability_v2_territory_availabilities_linkages_response_dict = app_availability_v2_territory_availabilities_linkages_response_instance.to_dict()
# create an instance of AppAvailabilityV2TerritoryAvailabilitiesLinkagesResponse from a dict
app_availability_v2_territory_availabilities_linkages_response_from_dict = AppAvailabilityV2TerritoryAvailabilitiesLinkagesResponse.from_dict(app_availability_v2_territory_availabilities_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


