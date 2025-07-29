# AppPriceScheduleManualPricesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppPriceScheduleRelationshipsManualPricesDataInner]**](AppPriceScheduleRelationshipsManualPricesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_price_schedule_manual_prices_linkages_response import AppPriceScheduleManualPricesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppPriceScheduleManualPricesLinkagesResponse from a JSON string
app_price_schedule_manual_prices_linkages_response_instance = AppPriceScheduleManualPricesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppPriceScheduleManualPricesLinkagesResponse.to_json())

# convert the object into a dict
app_price_schedule_manual_prices_linkages_response_dict = app_price_schedule_manual_prices_linkages_response_instance.to_dict()
# create an instance of AppPriceScheduleManualPricesLinkagesResponse from a dict
app_price_schedule_manual_prices_linkages_response_from_dict = AppPriceScheduleManualPricesLinkagesResponse.from_dict(app_price_schedule_manual_prices_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


