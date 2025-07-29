# TerritoryAvailabilityUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**TerritoryAvailabilityUpdateRequestDataAttributes**](TerritoryAvailabilityUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.territory_availability_update_request_data import TerritoryAvailabilityUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of TerritoryAvailabilityUpdateRequestData from a JSON string
territory_availability_update_request_data_instance = TerritoryAvailabilityUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(TerritoryAvailabilityUpdateRequestData.to_json())

# convert the object into a dict
territory_availability_update_request_data_dict = territory_availability_update_request_data_instance.to_dict()
# create an instance of TerritoryAvailabilityUpdateRequestData from a dict
territory_availability_update_request_data_from_dict = TerritoryAvailabilityUpdateRequestData.from_dict(territory_availability_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


