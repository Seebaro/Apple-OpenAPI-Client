# AppPriceScheduleCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app** | [**AccessibilityDeclarationCreateRequestDataRelationshipsApp**](AccessibilityDeclarationCreateRequestDataRelationshipsApp.md) |  | 
**base_territory** | [**AppPriceScheduleCreateRequestDataRelationshipsBaseTerritory**](AppPriceScheduleCreateRequestDataRelationshipsBaseTerritory.md) |  | 
**manual_prices** | [**AppPriceScheduleCreateRequestDataRelationshipsManualPrices**](AppPriceScheduleCreateRequestDataRelationshipsManualPrices.md) |  | 

## Example

```python
from openapi_client.models.app_price_schedule_create_request_data_relationships import AppPriceScheduleCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppPriceScheduleCreateRequestDataRelationships from a JSON string
app_price_schedule_create_request_data_relationships_instance = AppPriceScheduleCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(AppPriceScheduleCreateRequestDataRelationships.to_json())

# convert the object into a dict
app_price_schedule_create_request_data_relationships_dict = app_price_schedule_create_request_data_relationships_instance.to_dict()
# create an instance of AppPriceScheduleCreateRequestDataRelationships from a dict
app_price_schedule_create_request_data_relationships_from_dict = AppPriceScheduleCreateRequestDataRelationships.from_dict(app_price_schedule_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


