# AppPricesV2ResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**TerritoryAttributes**](TerritoryAttributes.md) |  | [optional] 
**relationships** | [**AppPricePointV3Relationships**](AppPricePointV3Relationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_prices_v2_response_included_inner import AppPricesV2ResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppPricesV2ResponseIncludedInner from a JSON string
app_prices_v2_response_included_inner_instance = AppPricesV2ResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppPricesV2ResponseIncludedInner.to_json())

# convert the object into a dict
app_prices_v2_response_included_inner_dict = app_prices_v2_response_included_inner_instance.to_dict()
# create an instance of AppPricesV2ResponseIncludedInner from a dict
app_prices_v2_response_included_inner_from_dict = AppPricesV2ResponseIncludedInner.from_dict(app_prices_v2_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


