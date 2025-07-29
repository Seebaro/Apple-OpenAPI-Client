# TerritoryAvailabilityUpdateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** |  | [optional] 
**release_date** | **date** |  | [optional] 
**pre_order_enabled** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.territory_availability_update_request_data_attributes import TerritoryAvailabilityUpdateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of TerritoryAvailabilityUpdateRequestDataAttributes from a JSON string
territory_availability_update_request_data_attributes_instance = TerritoryAvailabilityUpdateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(TerritoryAvailabilityUpdateRequestDataAttributes.to_json())

# convert the object into a dict
territory_availability_update_request_data_attributes_dict = territory_availability_update_request_data_attributes_instance.to_dict()
# create an instance of TerritoryAvailabilityUpdateRequestDataAttributes from a dict
territory_availability_update_request_data_attributes_from_dict = TerritoryAvailabilityUpdateRequestDataAttributes.from_dict(territory_availability_update_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


