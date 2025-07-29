# InAppPurchasePricePoint


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppPricePointV3Attributes**](AppPricePointV3Attributes.md) |  | [optional] 
**relationships** | [**InAppPurchasePricePointRelationships**](InAppPurchasePricePointRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_price_point import InAppPurchasePricePoint

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePricePoint from a JSON string
in_app_purchase_price_point_instance = InAppPurchasePricePoint.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePricePoint.to_json())

# convert the object into a dict
in_app_purchase_price_point_dict = in_app_purchase_price_point_instance.to_dict()
# create an instance of InAppPurchasePricePoint from a dict
in_app_purchase_price_point_from_dict = InAppPurchasePricePoint.from_dict(in_app_purchase_price_point_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


