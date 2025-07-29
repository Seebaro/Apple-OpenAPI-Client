# AppPriceScheduleAutomaticPricesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppPriceScheduleRelationshipsManualPricesDataInner]**](AppPriceScheduleRelationshipsManualPricesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_price_schedule_automatic_prices_linkages_response import AppPriceScheduleAutomaticPricesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppPriceScheduleAutomaticPricesLinkagesResponse from a JSON string
app_price_schedule_automatic_prices_linkages_response_instance = AppPriceScheduleAutomaticPricesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppPriceScheduleAutomaticPricesLinkagesResponse.to_json())

# convert the object into a dict
app_price_schedule_automatic_prices_linkages_response_dict = app_price_schedule_automatic_prices_linkages_response_instance.to_dict()
# create an instance of AppPriceScheduleAutomaticPricesLinkagesResponse from a dict
app_price_schedule_automatic_prices_linkages_response_from_dict = AppPriceScheduleAutomaticPricesLinkagesResponse.from_dict(app_price_schedule_automatic_prices_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


