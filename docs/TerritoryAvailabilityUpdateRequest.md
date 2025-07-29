# TerritoryAvailabilityUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**TerritoryAvailabilityUpdateRequestData**](TerritoryAvailabilityUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.territory_availability_update_request import TerritoryAvailabilityUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TerritoryAvailabilityUpdateRequest from a JSON string
territory_availability_update_request_instance = TerritoryAvailabilityUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(TerritoryAvailabilityUpdateRequest.to_json())

# convert the object into a dict
territory_availability_update_request_dict = territory_availability_update_request_instance.to_dict()
# create an instance of TerritoryAvailabilityUpdateRequest from a dict
territory_availability_update_request_from_dict = TerritoryAvailabilityUpdateRequest.from_dict(territory_availability_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


