# AppPriceScheduleRelationshipsManualPrices


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppPriceScheduleRelationshipsManualPricesDataInner]**](AppPriceScheduleRelationshipsManualPricesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_price_schedule_relationships_manual_prices import AppPriceScheduleRelationshipsManualPrices

# TODO update the JSON string below
json = "{}"
# create an instance of AppPriceScheduleRelationshipsManualPrices from a JSON string
app_price_schedule_relationships_manual_prices_instance = AppPriceScheduleRelationshipsManualPrices.from_json(json)
# print the JSON string representation of the object
print(AppPriceScheduleRelationshipsManualPrices.to_json())

# convert the object into a dict
app_price_schedule_relationships_manual_prices_dict = app_price_schedule_relationships_manual_prices_instance.to_dict()
# create an instance of AppPriceScheduleRelationshipsManualPrices from a dict
app_price_schedule_relationships_manual_prices_from_dict = AppPriceScheduleRelationshipsManualPrices.from_dict(app_price_schedule_relationships_manual_prices_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


