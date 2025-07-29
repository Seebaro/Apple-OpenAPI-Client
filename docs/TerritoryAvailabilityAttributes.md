# TerritoryAvailabilityAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** |  | [optional] 
**release_date** | **date** |  | [optional] 
**pre_order_enabled** | **bool** |  | [optional] 
**pre_order_publish_date** | **date** |  | [optional] 
**content_statuses** | **List[str]** |  | [optional] 

## Example

```python
from openapi_client.models.territory_availability_attributes import TerritoryAvailabilityAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of TerritoryAvailabilityAttributes from a JSON string
territory_availability_attributes_instance = TerritoryAvailabilityAttributes.from_json(json)
# print the JSON string representation of the object
print(TerritoryAvailabilityAttributes.to_json())

# convert the object into a dict
territory_availability_attributes_dict = territory_availability_attributes_instance.to_dict()
# create an instance of TerritoryAvailabilityAttributes from a dict
territory_availability_attributes_from_dict = TerritoryAvailabilityAttributes.from_dict(territory_availability_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


