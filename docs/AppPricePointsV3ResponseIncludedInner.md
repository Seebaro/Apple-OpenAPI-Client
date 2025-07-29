# AppPricePointsV3ResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**TerritoryAttributes**](TerritoryAttributes.md) |  | [optional] 
**relationships** | [**AppRelationships**](AppRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_price_points_v3_response_included_inner import AppPricePointsV3ResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppPricePointsV3ResponseIncludedInner from a JSON string
app_price_points_v3_response_included_inner_instance = AppPricePointsV3ResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppPricePointsV3ResponseIncludedInner.to_json())

# convert the object into a dict
app_price_points_v3_response_included_inner_dict = app_price_points_v3_response_included_inner_instance.to_dict()
# create an instance of AppPricePointsV3ResponseIncludedInner from a dict
app_price_points_v3_response_included_inner_from_dict = AppPricePointsV3ResponseIncludedInner.from_dict(app_price_points_v3_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


