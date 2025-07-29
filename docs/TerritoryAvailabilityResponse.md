# TerritoryAvailabilityResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**TerritoryAvailability**](TerritoryAvailability.md) |  | 
**included** | [**List[Territory]**](Territory.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.territory_availability_response import TerritoryAvailabilityResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TerritoryAvailabilityResponse from a JSON string
territory_availability_response_instance = TerritoryAvailabilityResponse.from_json(json)
# print the JSON string representation of the object
print(TerritoryAvailabilityResponse.to_json())

# convert the object into a dict
territory_availability_response_dict = territory_availability_response_instance.to_dict()
# create an instance of TerritoryAvailabilityResponse from a dict
territory_availability_response_from_dict = TerritoryAvailabilityResponse.from_dict(territory_availability_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


