# AppPriceScheduleBaseTerritoryLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppPricePointV3RelationshipsTerritoryData**](AppPricePointV3RelationshipsTerritoryData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_price_schedule_base_territory_linkage_response import AppPriceScheduleBaseTerritoryLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppPriceScheduleBaseTerritoryLinkageResponse from a JSON string
app_price_schedule_base_territory_linkage_response_instance = AppPriceScheduleBaseTerritoryLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppPriceScheduleBaseTerritoryLinkageResponse.to_json())

# convert the object into a dict
app_price_schedule_base_territory_linkage_response_dict = app_price_schedule_base_territory_linkage_response_instance.to_dict()
# create an instance of AppPriceScheduleBaseTerritoryLinkageResponse from a dict
app_price_schedule_base_territory_linkage_response_from_dict = AppPriceScheduleBaseTerritoryLinkageResponse.from_dict(app_price_schedule_base_territory_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


