# TerritoryAvailabilitiesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[TerritoryAvailability]**](TerritoryAvailability.md) |  | 
**included** | [**List[Territory]**](Territory.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.territory_availabilities_response import TerritoryAvailabilitiesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TerritoryAvailabilitiesResponse from a JSON string
territory_availabilities_response_instance = TerritoryAvailabilitiesResponse.from_json(json)
# print the JSON string representation of the object
print(TerritoryAvailabilitiesResponse.to_json())

# convert the object into a dict
territory_availabilities_response_dict = territory_availabilities_response_instance.to_dict()
# create an instance of TerritoryAvailabilitiesResponse from a dict
territory_availabilities_response_from_dict = TerritoryAvailabilitiesResponse.from_dict(territory_availabilities_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


