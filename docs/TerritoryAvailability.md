# TerritoryAvailability


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**TerritoryAvailabilityAttributes**](TerritoryAvailabilityAttributes.md) |  | [optional] 
**relationships** | [**CustomerReviewSummarizationRelationships**](CustomerReviewSummarizationRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.territory_availability import TerritoryAvailability

# TODO update the JSON string below
json = "{}"
# create an instance of TerritoryAvailability from a JSON string
territory_availability_instance = TerritoryAvailability.from_json(json)
# print the JSON string representation of the object
print(TerritoryAvailability.to_json())

# convert the object into a dict
territory_availability_dict = territory_availability_instance.to_dict()
# create an instance of TerritoryAvailability from a dict
territory_availability_from_dict = TerritoryAvailability.from_dict(territory_availability_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


