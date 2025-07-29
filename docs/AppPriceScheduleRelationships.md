# AppPriceScheduleRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app** | [**AlternativeDistributionKeyCreateRequestDataRelationshipsApp**](AlternativeDistributionKeyCreateRequestDataRelationshipsApp.md) |  | [optional] 
**base_territory** | [**AppPriceScheduleRelationshipsBaseTerritory**](AppPriceScheduleRelationshipsBaseTerritory.md) |  | [optional] 
**manual_prices** | [**AppPriceScheduleRelationshipsManualPrices**](AppPriceScheduleRelationshipsManualPrices.md) |  | [optional] 
**automatic_prices** | [**AppPriceScheduleRelationshipsManualPrices**](AppPriceScheduleRelationshipsManualPrices.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_price_schedule_relationships import AppPriceScheduleRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppPriceScheduleRelationships from a JSON string
app_price_schedule_relationships_instance = AppPriceScheduleRelationships.from_json(json)
# print the JSON string representation of the object
print(AppPriceScheduleRelationships.to_json())

# convert the object into a dict
app_price_schedule_relationships_dict = app_price_schedule_relationships_instance.to_dict()
# create an instance of AppPriceScheduleRelationships from a dict
app_price_schedule_relationships_from_dict = AppPriceScheduleRelationships.from_dict(app_price_schedule_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


