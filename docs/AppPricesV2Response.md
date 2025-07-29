# AppPricesV2Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppPriceV2]**](AppPriceV2.md) |  | 
**included** | [**List[AppPricesV2ResponseIncludedInner]**](AppPricesV2ResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_prices_v2_response import AppPricesV2Response

# TODO update the JSON string below
json = "{}"
# create an instance of AppPricesV2Response from a JSON string
app_prices_v2_response_instance = AppPricesV2Response.from_json(json)
# print the JSON string representation of the object
print(AppPricesV2Response.to_json())

# convert the object into a dict
app_prices_v2_response_dict = app_prices_v2_response_instance.to_dict()
# create an instance of AppPricesV2Response from a dict
app_prices_v2_response_from_dict = AppPricesV2Response.from_dict(app_prices_v2_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


