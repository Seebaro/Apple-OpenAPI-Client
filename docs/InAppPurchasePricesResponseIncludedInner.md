# InAppPurchasePricesResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**TerritoryAttributes**](TerritoryAttributes.md) |  | [optional] 
**relationships** | [**InAppPurchasePricePointRelationships**](InAppPurchasePricePointRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_prices_response_included_inner import InAppPurchasePricesResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePricesResponseIncludedInner from a JSON string
in_app_purchase_prices_response_included_inner_instance = InAppPurchasePricesResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePricesResponseIncludedInner.to_json())

# convert the object into a dict
in_app_purchase_prices_response_included_inner_dict = in_app_purchase_prices_response_included_inner_instance.to_dict()
# create an instance of InAppPurchasePricesResponseIncludedInner from a dict
in_app_purchase_prices_response_included_inner_from_dict = InAppPurchasePricesResponseIncludedInner.from_dict(in_app_purchase_prices_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


